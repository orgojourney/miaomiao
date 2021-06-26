<template>
  <div id="main">
    <Header title="喵喵电影"></Header>
    <div id="content">
      <div class="movie_menu">
        <div class="city_name">
         <router-link tag="li" to="/movie/city">大连</router-link>
        </div>
        <div class="hot_switch">
           <router-link tag="li" to="/movie/nowplaying" class="hot_item">正在热映</router-link>
            <router-link tag="li" to="/movie/comingsoon" class="hot_item">即将上映</router-link>
        </div>
        <div class="search_entry">
            <router-link tag="li" to="/movie/search">搜索</router-link>
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
li{list-style: none;}
#content{ fLex:1; overflow:auto; margin-bottom: 50px; position: relative; display:flex; flex-direction:column;}
#content .movie_menu{ width: 100;height:45px; border-bottom:1px solid #ebebeb; display: flex;flex-direction:row; justify-content:space-between;}
.city_name{ margin-left: 20px; height:100%; line-height: 45px;}
.movie_menu .city_name.router-link-active{ color: #ef4238; border-bottom: 2px #ef4238 solid;}
.movie_menu .hot_switch{ display:flex; height:100%; line-height: 45px;} 
.movie_menu .hot_item{ font-size: 15px; line-height: 40px;coLor:#666; width:80pX; text-align:center; margin:0 12px;}
.movie_menu .hot_item.active{ color: #ef4238; border-bottom: 2px #ef4238 solid;}
.movie_menu .hot_item.router-link-active{ color: #ef4238; border-bottom: 2px #ef4238 solid;}
.movie_menu .search_entry{ margin-right:20px; height:100%; Line-height: 45px;}
.movie_menu .search_entry.active{ color: #ef4238; border-bottom: 2px #ef4238 solid;}
.movie_menu .search_entry.router-link-active{ color: #ef4238; border-bottom: 2px #ef4238 solid;}
.movie_menu .search_entry i{ font-size:24px;color:red;}
</style>