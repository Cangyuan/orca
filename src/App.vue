<template>
  <div id="app">
    <v-header></v-header>
    <router-view/>
    <v-footer></v-footer>
  </div>
</template>

<script>
import header from '@/components/header/header'
import footer from '@/components/footer/footer'
export default {
  name: 'app',
  components: {
    'v-header': header,
    'v-footer': footer
  },
  created () {
    this.$api.get('topics', null, r => {
      console.log(r)
    })
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
</style>
