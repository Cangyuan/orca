<template>
  <div class="header">
  	<header id="header-wrap">
  		<ul>
  			<li></li>
  			<li></li>
  			<li></li>
  			<li></li>
  			<li></li>
  			<li></li>
  		</ul>
  	  	<div class="top-bar">
  		    <div class="bar-wrap">
  		      <div class="chicken"><img src="./chicken.gif" alt=""></div>
  		      <div class="top-title">
  		        <h2>orca</h2>
  		        <span>逆戟 · 个人网站</span>
  		      </div>
  		      <div class="bar-main">
  		        <div class="nav-wrap">
  		          <nav>
  		          	<div class="small-nav">
  		          		<img src="images/nav.png" alt="">
  		          	</div>
  		          	<span class="head-me"><img src="./me.png" alt=""></span>
  		            <ul>
  		              <li><a href="#home">首页</a></li>
  		              <li><a href="#about">关于</a></li>
  		              <li><a href="#skill">技能</a></li>
  		              <li><a href="#foot">履历</a></li>
  		              <li><a href="#writing">作品</a></li>
  		              <li><a href="/">博客</a></li>
  		              <li><a href="#contact">联系</a></li>
  		            </ul>
  		          </nav>

  		        </div>
  		        <ul></ul>
  		      </div>
  		    </div>
  	  	</div>
  		<div class="loading_bar">
  		  	<img src="images/loading.gif" alt="">
  		</div>
  	</header>
  </div>
</template>

<script>
export default {
  name: 'header',
  data () {
    return {
      msg: 'header part'
    }
  },
  methods:{
    // navJump(id){
    
    // }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
/*navbar start*/
#header-wrap{
  position: fixed;
  width: 100%;
  top: 0;
  z-index: 9999;
}
#header-wrap>ul{
  display: table;
  width:100%;
  height: 10px;
}
#header-wrap>ul>li{
  display: table-cell;
  height: 100%;
}
#header-wrap>ul>li:nth-of-type(1){
  background: #f12f25;
}
#header-wrap>ul>li:nth-of-type(2){
  background: #ff9531;
}
#header-wrap>ul>li:nth-of-type(3){
  background: #efd21f;
}
#header-wrap>ul>li:nth-of-type(4){
  background: #aec534;
}
#header-wrap>ul>li:nth-of-type(5){
  background: #24a5db;
}
#header-wrap>ul>li:nth-of-type(6){
  background: #5830cb;
}
.head-me{
  float: right;
    height: 32px;
    display: block;
    padding: 4px 0;
    box-sizing:border-box;
    cursor: pointer;
}
.head-me>img{
  display: block;
  height: 24px;
  line-height: 32px;
}
.top-bar{
  width: 100%;
  padding: 5px 0;
  background: #000;
  color: #fff;
  position: relative;
}
.bar-wrap{
  width: 90%;
  margin: 0 auto;
  height: 32px;
}
.top-title{
  width: 40%;
  text-align: left;
  float: left;
  height: 32px;
}
.top-title>a{
  display: inline-block;
  line-height: 32px;
  padding: 0;
  margin: 0;
}
.top-title>a>img{
  width: 32px;
  margin-top: -3px;
  height: auto;
}
.top-title>h2{
  display: inline;
  font-size: 24px;
  letter-spacing: 1px;
  padding-right: 10px;
  padding-left: 6px
}
.top-title>span{
  display: inline-block;
  font-size: 12px;
  color: #ccc;
  letter-spacing: 1px;
}
.bar-main{
  width: 60%;
  float: right;
  text-align: right;
}
.nav-wrap{
  width: 100%;
  height: 32px;
  /*position: relative;*/
  /*overflow: hidden;*/
}
.nav-wrap>nav{
  width: 100%;
  height: 100%;
  float: right;
}
.small-nav{
  display: none;
}

.nav-wrap>nav>ul{
  display: table;
  float: right;
}
.nav-wrap>nav>ul>li{
  display: table-cell;
}
.nav-wrap>nav>ul>li>a{
  color: #fff;
  padding: 0 10px;
  font-size: 16px;
  position: relative;
  line-height: 32px;
  font-family: '微软雅黑';
  letter-spacing: 6px;
}
.nav-wrap>nav>ul>li>a:after{
  content: "*";
  display: block;
  right: -6px;
  font-size: 20px;
  line-height: 32px;
  color: #fff;
  font-size: 20px;
  position: absolute;
  top: -2px;
}
.navActive{
  color: #b4b4b4!important;
}
</style>
