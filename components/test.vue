<template>
  <div class="hello">Hello {{ who }} <comp></comp></div>
</template>

<script>
module.exports = {
  components: {
    comp: httpVueLoader("components/comp.vue"),
  },
  data: function () {
    return {
      who: "world",
    };
  },
};
</script>

<style>
.hello {
  background-color: #ffe;
}
</style>
