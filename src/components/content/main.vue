<template>
  <div class="main">
  	<div class="main-bg"></div>
  	<div class="info-wrap" id="home">
  	  <div class="info-bg">
  	    <div class="info-img">
  	      <img src="./logo-top.png" alt="">
  	    </div>
  	    <p>美景如画，四季如春</p> 
  	  </div>  
  	</div>
  	<section id="about">
  	    <div class="se-title ab-title">
  	      <h2>简介</h2>
  	      <span class="border"></span>
  	      <h4>profile</h4>
  	    </div>
  	    <div class="ab-content">
  	      <div class="wrap-me"><img src="./me.jpg" alt=""></div>
  	      <p><strong>orca</strong></p>
  	      <p>现居地 浙江<span>·</span>杭州</p>
  	      <p>web前端开发工程师</p>
  	      <p>新乡医学院<span>·</span>本科</p>
  	      <p>爱好<span>·</span>看书<span>·</span>跑步</p>
  	      <p>专注界面设计、交互设计、前端开发，关注互联</p>
  	    </div>
  	</section>
  	<v-skill></v-skill>
    <v-foot></v-foot>
    <v-writing></v-writing>
    <v-contact></v-contact>
  </div>
</template>

<script>
import skill from '@/components/skill/skill'
import foot from '@/components/foot/foot'
import writing from '@/components/writing/writing'
import contact from '@/components/contact/contact'
export default {
  name: 'main',
  components: {
    'v-skill': skill,
    'v-foot': foot,
    'v-writing': writing,
    'v-contact': contact
  },
  data () {
    return {
      // msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.main{
  position: relative;
}
.main-bg{
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  opacity: .8;
  background: #fff;
  z-index: 999;
  display: none;
  -ms-filter: "alpha(opacity=80)";
    filter: alpha(opacity=80);
    -webkit-transition: .01s opacity ease .2s;
    -moz-transition: .01s opacity ease .2s;
    -o-transition: .01s opacity ease .2s;
    -ms-transition: .01s opacity ease .2s;
    transition: .01s opacity ease .2s;
}
.info-wrap{
  height: 248px;
  background: url(./top-bg.jpg);
  background-size: 100% auto;
  background-position: center;
}
.info-bg{
  background: rgba(0,0,0,.7);
  width: 100%;
  height: 100%;
}
.info-img{
  padding-top: 60px;
  width: 100%;
  position: relative;
}
.info-img>img{
  display: block;
  width: 100px;
  margin: 15px auto;
}
.info-wrap p{
  color: #ccc;
  text-align: center;
  letter-spacing: 2px;
}
#about{
  padding: 30px 0;
  margin-bottom: 30px;
  position: relative;
  top: 0;
  -webkit-transition: all 2 ease;
  -moz-transition: all 2 ease;
  -ms-transition: all 2 ease;
  -o-transition: all 2 ease;
  transition: all 2 ease;
}
.ab-content{
  padding: 0 20%;
}
/*.onload{
  width: 100%;
  height: 100%;
}*/
.ab-content>p{
  text-align: center;
  color: #424242;
  padding: 6px 0;
}
.ab-content>p>span{
  padding: 2px 4px 0 4px;
  color: #1e1e34;
  font-weight: 400;
  font-size: 20px;
}
.ab-content>p:nth-of-type(1){
  font-size: 18px;
}
.wrap-me{
  width: 300px;
  height:300px;
  overflow: hidden;
  transform: rotate(-45deg);
  margin: 70px auto;
}
.wrap-me>img{
  width: 300px;
  height: 300px;
  transform: rotate(45deg) scale(1.38);
}


@media screen and (max-width: 890px){
  #skill, #foot, #writing, #contact{
    padding:0!important;  
  }
  .wr-title{
    padding-bottom: 0!important; 
  }
  #skill, #foot{
    padding-bottom: 40px!important; 
  }
  p{
    line-height: 1.6!important;    
  }
  .sk-co-title p,.sk-list li{
     font-size: .5rem!important;   
  }
  .info-wrap{
    background-size: cover!important;   
  }
  .se-title>h2{
    letter-spacing: .1rem!important;   
  }
  .se-title>span{
    width: 20%!important;   
  }
  .top-title>span{
    display: none!important;   
  }
  .ab-content>p{    
    padding: 0!important;   
  }
  #header-wrap{
    position: relative!important;  
    height:42px;
  }
  .wrap-me{
    width: 150px!important;   
    height: 150px!important;     
  }
  .wrap-me>img{
    width: 150px!important;   
    height: 150px!important;   
  }
  .sk-content>ul>li{
    display: block;
    width: 100%;
  }
  .wr-content>ul,.co-content>ul{
    display: flex!important;  
    width: 100%!important;  
    flex-flow: row wrap!important;  
    align-content: flex-start!important;  
  }
  .wr-content>ul>li,.co-content>ul>li{
    flex: 0 0 50%!important;  
    padding: 3%!important;  
    display: block!important;  
  }
  .co-content>ul>li{
    padding: 3% 0!important;  
  }
  .co-content>p{
    margin-bottom:10px!important; 
  }
  .w-txt>h3{
    font-size: .8rem!important;  
  }
  .nav-wrap>nav>ul{
    position: absolute!important;  
      top: 37px!important;  
      right: 0!important;  
      width: 100px!important;  
      z-index: 999!important;  
      background: #111!important;  
      display: none!important;  
  }
  .nav-wrap>nav>ul>li{
    display: block!important;  
    text-align: center!important;  
  }
  .small-nav{
    display: block!important;  
    height: 100%!important;  
    float: right!important;  
    margin-left: 4px!important;  
  }
  .small-nav>img{
    display: block!important;  
    height: 100%!important;  
    padding: 6px!important;  
    box-sizing: border-box!important;  
  }
  .info-wrap{
    height: 148px!important;  
  }
  .info-img{
    padding-top: 10px!important;  
  }
  .info-img>img{
    width: 60px!important;  
  }
  .wr-content{
    padding: 0
  }
}
</style>
