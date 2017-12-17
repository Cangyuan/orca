<template>
  <section id="contact" data-animation="flipInX" data-timeout="400">
    <div class="se-title">
      <h2>联系我</h2>
      <span class="border"></span>
      <h4>contact me</h4>
    </div>
    <div class="co-content">
      <p>欢迎合作及提供工作机会。</p>
      <ul>
        <li>
          <a href="http://wpa.qq.com/msgrd?v=3&uin=1339918746&site=qq&menu=yes" target="_blank">
            <i class="iconfont icon-qq"></i>
            <p>1339918746</p>
          </a>
        </li>
        <li>
          <a href="https://www.linkedin.com/in/orca2017/" target="_blank">
            <i class="iconfont icon-linkedin"></i>
            <p>@orca</p>
          </a>
        </li>
        <li>
          <a href="https://github.com/Cangyuan" target="_blank">
            <i class="iconfont icon-github"></i>
            <p>@cangyuan.github</p>
          </a>
        </li>
        <li>
          <a href="https://cangyuan.github.io">
            <i class="iconfont icon-blog"></i>
            <p>我的博客</p>
          </a>
        </li>
      </ul>
    </div>
  </section>
</template>
<script>
export default {
  name: 'contact',
  data () {
    return {
      // msg: 'header part'
    }
  }
}
</script>
<style>
  .co-content{
    padding: 10px;
    text-align: center;
    margin-bottom: 30px;
    
  }
  .co-content>p{
    font-size: 16px;
    margin-bottom: 50px;
    letter-spacing: 6px;
  }
  .co-content>ul{
    display: table;
    width: 80%;
    margin: 0 auto;
    padding: 30px 0;
  }
  .co-content>ul>li{
    display: table-cell;
    text-align: center;
    width: 25%;    
  }
  .co-content>ul>li>a{
    opacity: .4;
    color: #777;
    text-decoration: none;
  }
  .co-content>ul>li>a:hover{
    opacity: 1;
    color: #000
  }
  .co-content>ul>li>a>i{
    font-size: 42px;
    margin: 10px 0;
  }
</style>
