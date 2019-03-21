<template>
  <p class="hide">{{text_p}}</p>
</template>

<script>
// props的优先级 > data中的优先级 > menthods中的优先级
export default {
  // data() {
  //   return {
  //     text_p: "lllll"
  //   };
  // },
  props: ["text_p"]
};
</script>

<style>
.hide {
  display: none;
}
.show {
  display: block;
}
</style>


