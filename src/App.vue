<template>
  <div id="app">
    <v-me></v-me>
    <div class="wrap">
      <v-header></v-header>
      <router-view/>
      <v-footer></v-footer>
    </div>   
  </div>
</template>

<script>
import me from '@/components/me/me'
import header from '@/components/header/header'
import footer from '@/components/footer/footer'
export default {
  name: 'app',
  components: {
    'v-me': me,
    'v-header': header,
    'v-footer': footer
  },
  // created () {
  //   this.$api.get('topics', null, r => {
  //     console.log(r)
  //   })
  // },
  methods:{

  },
  mounted:function(){
    //滚动加载css3动画  
    $(window).scroll(function(){
      var a,b,c,con,foot,wr;
      con=$('.co-content').offset().top;
      foot=$('#foot').offset().top;
      wr=$('#writing').offset().top;
      a=eval(con + 100);
      b=$(window).scrollTop(); 
      c=$(window).height();
      if(b+c>a){
          $('.co-content>ul>li').addClass('scroll');
      }
      if(b+c>wr + 400){
           $('.wr-content>ul>li').addClass('fade');
      }
    }) 
    // 锚点跳转
    $('.nav-wrap>nav>ul>li>a').click(function(event) {
      /* Act on the event */
      var Id = $(this).attr('href');
      $("html,body").animate({scrollTop: $(Id).offset().top}, 1000);
    }); 
  }
}
</script>

<style>
#app{
  background-color: #f0f0f0;
}
#skill,#foot,#writing,#contact{
  padding: 40px 0;
  position: relative;
}
.wrap{
  position: relative;
  left: 0;
  -webkit-transition: all .3s ease;
  -moz-transition: all .3s ease;
  -ms-transition: all .3s ease;
  -o-transition: all .3s ease;
  transition: all .3s ease;
}
.remove{
  width: 100%;
  left: 266px;
  -webkit-transition: all .3s ease;
  -moz-transition: all .3s ease;
  -ms-transition: all .3s ease;
  -o-transition: all .3s ease;
  transition: all .3s ease;
}
/*me-info start*/
.open-me{
  opacity: 1!important;
  left: 0!important;
}
.me-info{
  position: fixed;
  left: -100%;
  top: 0;
  width: 266px;
  height: 100%;
  background: #000;
  color: #fff;
  padding: 30px 10px;
  box-sizing:border-box;
  -webkit-transition: all .3s ease;
  -moz-transition: all .3s ease;
  -ms-transition: all .3s ease;
  -o-transition: all .3s ease;
  transition: all .3s ease;
  opacity: 0;
}
.me-info>.me>.me-pic{
  width: 160px;
  height: 160px;
  display: block;
  margin: 0 auto;
  /*overflow: hidden;*/
  border-radius: 50%;
  box-shadow: 0 0 15px #f9e249;
  
}
.me-pic .me-wrap{
  width: 160px;
  height: 160px;
  display: block;
  overflow: hidden;
  border-radius: 50%;
  position: relative;
  z-index: 1;
}
.me-pic .me-wrap img:hover{
  transform: scale(2);
  transition: .5s;
}
.me-pic .me-wrap img{
  width: 100%;
  height: 100%;
  border-radius: 50%;
  transition: .5s;
}
.me-info>.me>h3{
  font-size: 18px;
  text-align: center;
  padding: 10px 0;
  margin-bottom: 10px;
}
.me-txt{
  text-indent: 28px;
  line-height: 1.6;
  padding: 0 10px;
  margin-bottom: 30px;
}
.detail{
  padding-left: 10px;
  text-align: left;
  text-indent: 0!important;
  line-height: 1.6;
  text-shadow: 2px 2px 2px #f6b6ab;
  letter-spacing: 1px;
  font-size: 16px;
}
.detail>a{
  color: #d4d4d4;
}
.close{
  position: absolute;
  top: 10px;
  right: 10px;
  color: #d6d6d6;
  font-size: 20px;
  cursor: pointer;
}
.se-title{
  padding: 50px 0;
}
.se-title>h2,.se-title>span,.se-title>h4{
  text-align: center;
  letter-spacing: .1rem;
}
.se-title>h2{
  letter-spacing: .5rem;
  font-size: 18px
}
.se-title>span{
  display: block;
  width: 10%;
  height: 2px;
  background: #871a04;
  margin: 14px auto;
}
.se-title>h4{
  text-transform: uppercase;
  font-size: 16px;
}
.scroll{
  -webkit-animation-name: entrance;
  -moz-animation-name: entrance;
  -o-animation-name: entrance;
  animation-name: entrance;
  -webkit-animation-duration: 1.6s;
  -moz-animation-duration: 1.6s;
  -ms-animation-duration: 1.6s;
  -o-animation-duration: 1.6s;
  animation-duration: 1.6s;
  opacity: 1 !important;

  -webkit-animation-fill-mode: both;
  -moz-animation-fill-mode: both;
  -ms-animation-fill-mode: both;
  -o-animation-fill-mode: both;
  animation-fill-mode: both;
  -webkit-animation-delay: .3s;
  -moz-animation-delay: .3s;
  animation-delay: .3s;
}

@keyframes bg{
  0% {
      -moz-transform: translate3d(0,0,0);
      -webkit-transform: translate3d(0,0,0);
      -o-transform: translate3d(0,0,0);
      -ms-transform: translate3d(0,0,0);
      transform: translate3d(0,0,0);
  }
  100% {
      -moz-transform: translate3d(-1200px,0,0);
      -webkit-transform: translate3d(-1200px,0,0);
      -o-transform: translate3d(-1200px,0,0);
      -ms-transform: translate3d(-1200px,0,0);
      transform: translate3d(-1200px,0,0);
  }
}
@keyframes entrance{
  0% {
      transform: scale(0.3) rotate(6deg) translateX(-30%) translateY(30%);
      opacity: .2;
  }
  30% {
      transform: scale(1.03) rotate(-2deg) translateX(2%) translateY(-2%);
      opacity: 1;
  }
  45% {
      transform: scale(0.98) rotate(1deg) translateX(0%) translateY(0%);
      opacity: 1;
  }
  60% {
      transform: scale(1.01) rotate(-1deg) translateX(0%) translateY(0%);
      opacity: 1;
  }
  75% {
      transform: scale(0.99) rotate(1deg) translateX(0%) translateY(0%);
      opacity: 1;
  }
  90% {
      transform: scale(1.01) rotate(0deg) translateX(0%) translateY(0%);
      opacity: 1;
  }

  100% {
      transform: scale(1) rotate(0deg) translateX(0%) translateY(0%);
      opacity: 1;
  }
}
</style>
