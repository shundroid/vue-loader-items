<style>
 .red {
   color: #f00;
 }
</style>

<template>
  <div>
    <hoge v-for="item in items" :msg="item.a"></hoge>
  </div>
</template>

<script>
var model = require("./model");
module.exports = {
  data: function() {
    return {
      items: model.state.items
    };
  },
  components: {
    hoge: require("./hoge.vue")
  }
};
</script>
