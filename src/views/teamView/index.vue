<!--
 * @Author: Chai chai 2787922490@qq.com
 * @Date: 2022-11-09 20:41:58
 * @LastEditors: Chai chai 2787922490@qq.com
 * @LastEditTime: 2023-02-23 14:35:18
 * @FilePath: \4433studio\src\views\teamView\index.vue
 * @Description: 
 * 
 * Copyright (c) 2022 by Chai chai 2787922490@qq.com, All Rights Reserved. 
-->

<template>
  <div class="bB">
    <div class="teamTitle">TEAM OF US</div>
    <!-- 卡片 -->
    <div class="cardBox">
      <cardView
        v-for="(user, index) in teams"
        :key="index"
        :name="user.name"
        :tags="user.tags"
        :selfContent="user.selfContent"
        :imgUrl="user.imgUrl"
      ></cardView>
    </div>
  </div>
</template>

<script>
import cardView from "@/components/cardView/index.vue";
export default {
  components: { cardView },
  data: () => {
    return {
      teams: [
        {
          name: "柴柴",
          tags: ["前端负责人", "前端工程师", "工作室负责人"],
          selfContent:
            "vue二次元个人博客模板作者，热爱花里胡哨的开发，涉猎广泛，励志做一名优秀的、花里胡哨的程序员",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/chaichai.jpg",
        },
        {
          name: "张三同学",
          tags: ["前端工程师", "前端副负责人", "工作室副负责人"],
          selfContent:
            "爱搞事的闲散青年，兴趣广泛，善于行动，热爱生活，立志成为一名18线全栈攻城狮，我的城科微信小程序作者。",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/zs.jpg",
        },
        {
          name: "土豆",
          tags: ["后端负责人", "后端工程师"],
          selfContent: "给你最完美的数据就是return True",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/td.jpg",
        },
        {
          name: "旧颜",
          tags: ["后端副负责人", "后端工程师"],
          selfContent: "立志成为一个十八线后端程序员！",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/jy.png",
        },
        {
          name: "百梦",
          tags: ["首席架构师"],
          selfContent: "我是蠢狗",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/bm.jpg",
        },
        {
          name: "鲨鲨",
          tags: ["后端工程师"],
          selfContent: "无所谓，我会出手",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/ss.jpg",
        },
        {
          name: "屁屁",
          tags: ["UI设计师"],
          selfContent: "我也是蠢狗",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/pp.jpg",
        },
        {
          name: "渣男",
          tags: ["后端工程师"],
          selfContent: "我真的想让这个世界变得更好，但是他们不给我源代码……",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/zn.png",
        },
        {
          name: "轩轩",
          tags: ["后端工程师"],
          selfContent: "代码乱得只有自己能看懂，公司不可替代的重要人才",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/yz.jpg",
        },
        {
          name: "墨卿",
          tags: ["前端工程师"],
          selfContent: "每次npm run 就像开奖,见红直接开摆",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/mm.jpg",
        },
        {
          name: "小七",
          tags: ["前端工程师"],
          selfContent: "是个前端，开发练习两年半只会v2，v3学习中",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/xq.jpg",
        },
        {
          name: "斯普努尔",
          tags: ["前端工程师"],
          selfContent: "春恨秋悲皆自惹，bugbug快走开",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/qpne.jpg",
        },
        {
          name: "SAO2233",
          tags: ["前端工程师"],
          selfContent: "react，vue",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/SAO2233.jpg",
        },
        {
          name: "渡渡",
          tags: ["UI设计师"],
          selfContent: "在梭哈了！！！",
          imgUrl:
            "https://4433studio.oss-cn-hangzhou.aliyuncs.com/headPortrait/dd.jpg",
        },
      ],
    };
  },
};
</script>

<style>
.bB {
  overflow: hidden;
}
.teamTitle {
  font-weight: 550;
  font-size: 30px;
  margin-top: 50px;
  margin-bottom: 60px;
  text-align: center;
}
.cardBox {
  width: 70vw;
  /* height: 80vh; */
  display: flex;
  margin: 0 auto;
  flex-wrap: wrap;
}
</style>
