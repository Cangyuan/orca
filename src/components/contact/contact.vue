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
            <img src="./QQ.png" alt="1339918746">
            <p>1339918746</p>
          </a>
        </li>
        <li>
          <a href="https://twitter.com/Orca_2017" target="_blank">
            <img src="./twitter.png" alt="orca">
            <p>@orca</p>
          </a>
        </li>
        <li>
          <a href="https://github.com/Cangyuan" target="_blank">
            <img src="./github.png" alt="cangyuan" title="cangyuan">
            <p>@cangyuan.github</p>
          </a>
        </li>
        <li>
          <a href="Mailto:orca2017@sina.cn">
            <img src="./email.png" alt="邮件" title="邮件">
            <p>orca2017@sina.cn</p>
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
  }
  .co-content>ul>li>a:hover{
    opacity: 1;
    color: #000
  }
  .co-content>ul>li>a>img{
    width: 40px;
    margin: 10px 0;
  }
</style>
