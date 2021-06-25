<template>
  <div id="main">
    <Header title="喵喵电影"></Header>
    <div id="content">
      <div class="movie_menu">
        <div class="city_name">
          <span>大连</span><i class="iconfont icon-lower-triangle"></i>
        </div>
        <div class="hot_switch">
            <div class="hot_item active">正在热映</div>
            <div class="hot_item">即将上映</div>
        </div>
        <div class="search_entry">
            <i class="iconfont icon-sousuo">搜索</i>
        </div>
      </div>
      <keep-alive>
          <router-view></router-view>
      </keep-alive>
    </div>
    <Tabber></Tabber>
  </div>
</template>

<script>
import Header from "@/components/Header";
import Tabber from "@/components/Tabber";

export default {
  name: "Movie",
  components: {
    Header,
    Tabber,
  },
};
</script>

<style scoped>
#content{ fLex:1; overflow:auto; margin-bottom: 50px; position: relative; display:flex; flex-direction:column;}
#content .movie_menu{ width: 100;height:45px; border-bottom:1px solid #ebebeb; display: flex; justify-content:space-between;}
.city_name{ margin-left: 20px; height:100%; line-height: 45px;}
.movie_menu .city_name.active{ color: #ef4238; border-bottom: 2px #ef4238 solid;}
.movie_menu .hot_swtich{ display:flex; height:100%; line-height: 45px;}
.movie_menu .hot_item{ font-size: 15px; coLor:#666; width:80pX; text-align:center; margin:0 12px; font-weight:70.}
.movie_menu .hot_item.active{ color: #ef4238; border-bottom: 2px #ef4238 solid;}
.movie_menu .search_entry{ margin-right:20px; height:100%; Line-height: 45px;}
.movie_menu .search_entry.active{ color: #ef4238; border-bottom: 2px #ef4238 solid;}
.movie_menu .search_entry i{ font-size:24px;color:red;}
</style>