<template>
  <div class="header">
    <router-link :to="{path: '/'}" class="logo">
      <img src="../../dist/logo.png" alt="Mss" width="100" height="47">
    </router-link>
    <div class="nav">
      <ul>
        <li>
          <router-link :to="{path: '/project'}">项目</router-link>
        </li>
        <!-- <li>
          <router-link :to="{path: '/photography'}">摄影</router-link>
        </li> -->
        <li>
          <router-link :to="{path: '/message'}">留言</router-link>
        </li>
        <li>
          <a href="https://github.com/Maxiaoxiang" target="_blank">Github</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style lang="scss" scope>
.header {
  display: inline-flex;
  justify-content: space-between;
  flex: 0 0 auto;
  position: fixed;
  line-height: 80px;
  font-size: 24px;
  box-sizing: border-box;
  background: #fff;
  width: calc(100% - 52px);
  z-index: 99;
  border-bottom: 1px solid #f1f1f1;
  box-shadow: -1px -1px 5px 2px #e6e6e6;
  .logo {
    margin-left: 32px;
    font-size: 0;
  }
  .nav {
    ul {
      display: inline-flex;
    }
    li {
      margin-right: 16px;
      font-weight: bold;
    }
    a {
      padding: 0 16px;
    }
  }
}
</style>
