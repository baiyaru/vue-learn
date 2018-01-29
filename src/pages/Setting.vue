<!-- 模板：html结构 -->
<template>
  <div>
    <mt-header fixed :title="title" class="title">
      <router-link :to="{path: '/', meta: {tab: 'tab4'}}" slot="left">
        <mt-button icon="back"></mt-button>
        <!--<mt-button @click="handleClose">我</mt-button>-->
      </router-link>
    </mt-header>
    <div class="">
      <div class="list">
        <mt-cell title="账户与安全" is-link ></mt-cell>
      </div>
      <div class="list">
        <mt-cell title="实名认证" is-link ></mt-cell>
        <mt-cell title="车主认证" is-link ></mt-cell>
      </div>
      <div class="list">
        <mt-cell title="我的地址" is-link ></mt-cell>
      </div>
      <div class="list">
        <mt-cell title="法律条款" is-link ></mt-cell>
        <mt-cell title="关于我们" is-link ></mt-cell>
      </div>
    </div>
  </div>
</template>

<!-- 行为：处理逻辑-->
<script>
  import { MessageBox } from 'mint-ui';

  export default {
    name: "Setting",
    data() {
      return {
        title: "設置"
      }
    }
  }


</script>

<!-- 样式：界面样式 -->
<style scoped>

  .title {
    height: 44px;
    font-size: 18px;
    color: #fff;
    background-color: #333;
  }

</style>
