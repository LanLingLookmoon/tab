<template>
  <div>
    <div class="tab">
      <!-- click不加.native会以为是自定义事件，因此要加.native告诉vue是原生点击事件 -->
      <tab-item
        v-for="(list,index) in lists"
        :key="index"
        :itemTitle="list.title"
        :class="{active: actived == index}"
        @click.native="change(index)"
      ></tab-item>
    </div>
    <pages
      v-for="(list,index) in lists"
      :key="index"
      :text_p="list.text"
      :class="{show: actived == index}"
    ></pages>
  </div>
</template>

<script>
// 引入地址
import tabItem from "../tabitem";
import pages from "../pages";
export default {
  components: {
    pages,
    tabItem
  },
  // 数据
  data() {
    return {
      actived: 0,
      lists: [
        {
          title: "11111",
          text: "11111"
        },
        {
          title: "2222",
          text: "22222"
        },
        {
          title: "3333",
          text: "33333"
        },
        {
          title: "4444",
          text: "44444"
        }
      ]
    };
  },
  methods: {
    change(index) {
      this.actived = index;
    }
  }
};
</script>
<style>
.tab {
  width: 100%;
  display: flex;
}
</style>

