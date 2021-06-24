<template>
  <footer id="footer">
    <ul>
      <router-link tag="li" to="/movie">
        <i class="iconfont icon-dianying"></i>
        <p>电影</p>
      </router-link>
      <router-link tag="li" to="/cinema">
        <i class="iconfont icon-yingyuan"></i>
        <p>影院</p>
      </router-link>
      <router-link tag="li" to="/mine">
        <i class="iconfont icon-wode"></i>
        <p>我的</p>
      </router-link>
    </ul>
  </footer>
</template>

<script>
export default {
  name: "Tabber",
};
</script>

<style scoped>
li{ list-style: none;}
#footer{width: 100%; height: 50px; background-color: #fff; border-top: 2px #9999ff solid; position: fixed; left: 0; bottom: 0;}
#footer ul{ display: flex; text-align: center; height: 50px; align-items: center; background-image: linear-gradient(120deg, #e0c3fc 0%, #8ec5fc 100%);}
#footer ul li{flex: 1; height: 40px; color: #00ffcc;}
#footer ul li.router-link-active{color: #9999ff;}
#footer ul i{font-size: 20px;}
#footer ul p{font-size: 12px; line-height: 50px; }
</style>