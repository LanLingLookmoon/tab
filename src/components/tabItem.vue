<template>
  <div class="tab-item">{{itemTitle}}</div>
</template>

<script>
export default {
  props: ["itemTitle"]
};
</script>


<style>
.tab-item {
  line-height: 40px;
  text-align: center;
  background-color: rgb(241, 82, 82);
  flex: 1;
}
.active {
  background-color: #000;
  color: rgb(241, 82, 82);
}
</style>

