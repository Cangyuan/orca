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
  	      <p>现居地 广东<span>·</span>佛山</p>
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
      msg: 'Welcome to Your Vue.js App'
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
</style>
