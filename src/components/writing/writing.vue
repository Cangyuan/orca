<template>
	<section id="writing">
  	  <div class="se-title wr-title">
  	    <h2>作品</h2>
  	    <span class="border"></span>
  	    <h4>my works</h4>
  	  </div>
  	  <div class="wr-content">
  	    <ul>
  	      <li>
  	        <a class="w-link" href="http://www.gdchenyi.com.cn" target="_blank">
  	          <div class="wr-img">
  	            <img src="./cy.jpg" alt="辰宜">
  	          </div>
  	          <div class="w-txt">
  	          	<h3>广东辰宜信息科技官网</h3>
  	          	<p><strong>开发时间:</strong>2016年4月</p>
  	          	<p><strong>工作详情:</strong>响应式布局PC端和移动端，运用 angular+jqurey+java进行前端UI布局以及
开发工作。</p>
  	          </div>
  	        </a>
  	      </li>
  	      <li>
  	      	<a class="w-link" href="javascript:;" target="_blank">
  		        <div class="wr-img">
  		          <img src="./nanhai-home.jpg" alt="辰宜">
  		        </div>
  		        <div class="w-txt">
  		        	<h3>南海区一窗通办填表系统</h3>
  		        	<p><strong>开发时间:</strong>2016年6月</p>
  		        	<p><strong>工作详情:</strong>根据设计效果图完成psd切图,DIV/CSS布局， JavaScript效果渲染、与后台接口对接等前端相关的开发工作。</p>
  		        </div>
  		    </a>
  	      </li>
  	      <li>
  	      	<a class="w-link" href="javascript:;" target="_blank">
  		        <div class="wr-img">
  		          <img src="./psAr.jpg" alt="orca个人博客">
  		        </div>
  		        <div class="w-txt">
  		        	<h3>我的博客</h3>
  		        	<!-- <p><strong>开发时间:</strong>2015年11月</p> -->
  		        	<p><strong>详情:</strong>github+hexo+git搭建自主博客</p>
  		        </div>
  		    </a>
  	      </li>
  	      <li>
  		      <a class="w-link" href="/sell" target="_blank">
  		        <div class="wr-img">
  		          <img src="./qi.jpg" alt="饿了么">
  		        </div>
  		        <div class="w-txt">
  		        	<h3>仿饿了么平台</h3>
  		        	<!-- <p><strong>开发时间:</strong>2015年11月</p> -->
  		        	<p><strong>工作详情:</strong>node+vue2+vue-router+axois+sass构建商品页，商家页面，购物页面等</p>
  		        </div>
  		      </a>
  	      </li>
  	      
  	    </ul>
  	  </div>
  	</section>
</template>
<script>
export default {
  name: 'foot',
  data () {
    return {
      // msg: 'header part'
    }
  }
}
</script>
<style>
	#writing{
		position: relative;
		overflow: hidden;
		padding:0;
	}
	#writing:before{
		content: '';
		display: block;
		background-size: auto 100%;
		position: absolute;
		left: 0;
		top: 0;
		width: 3600px;
		height: 100%;
		background: url(./writing-bg.jpg);
		background-position: bottom left;
		background-repeat: repeat-x;
		moz-animation: bg 60s linear infinite;
	    -webkit-animation: bg 60s linear infinite;
	    -o-animation: bg 60s linear infinite;
	    -ms-animation: bg 60s linear infinite;
	    animation: bg 60s linear infinite;
	    -moz-backface-visibility: hidden;
	    -moz-transform: translate3d(0,0,0);
	    -webkit-transform: translate3d(0,0,0);
	    -o-transform: translate3d(0,0,0);
	    -ms-transform: translate3d(0,0,0);
	    transform: translate3d(0,0,0);
	}
	#writing{
		
	}
	.wr-content{
		position: relative;
		z-index: 99;
		padding: 30px 0;
		padding-bottom: 50px;
		width: 90%;
		margin: 0 auto;
	}
	.event_wrap{
		/*transform: rotate(-90deg);*/
		/*transform: ;*/
	}
	.wr-title{
		position: relative;
		z-index: 100;
		color: #fff;
	}
	.wr-content>ul{
		display: table;
	}
	.wr-content>ul>li{
		display: table-cell;
		width: 25%;
		padding: 1%;
		box-sizing:border-box;
		position: relative;
		left: 20px;
		top: 40px;
		opacity: 0;
		-webkit-transition: all 1s ease-in;
	    -moz-transition: all 1s ease-in;
	    -ms-transition: all 1s ease-in;
	    -o-transition: all 1s ease-in;
	    transition: all 1s ease-in;
	}
	.wr-content>ul>li.fade{
		top: 0;
		left: 0;
		opacity: 1;
		-webkit-transition: all 1s ease-in;
	    -moz-transition: all 1s ease-in;
	    -ms-transition: all 1s ease-in;
	    -o-transition: all 1s ease-in;
	    transition: all 1s ease-in;
	}
	.wr-content>ul>li:nth-of-type(even){
		-webkit-transition: all 1.5s ease-in;
	    -moz-transition: all 1.5s ease-in;
	    -ms-transition: all 1.5s ease-in;
	    -o-transition: all 1.5s ease-in;
	    transition: all 1.5s ease-in;
	}
	.wr-img{
		width: 100%;	
	}
	.w-link{
		display: block;
		width: 100%;
		height: 100%;
		box-shadow: 2px 2px 2px #959595,4px 4px 2px #959595;
		position: relative;
		overflow: hidden;
	}
	.wr-img>img{
		width: 100%;
		-webkit-transform: scale(1);
	    -moz-transform: scale(1);
	    -ms-transform: scale(1);
	    -o-transform: scale(1);
	    transform: scale(1);
	    -webkit-transition: all 0.2s ease-in;
	    -moz-transition: all 0.2s ease-in;
	    -ms-transition: all 0.2s ease-in;
	    -o-transition: all 0.2s ease-in;
	    transition: all 0.2s ease-in;
	}
	.w-txt{
		position: absolute;
		top: 100%;
		left: 0;
		width: 100%;
		height: 100%;
		color: #fff;
		/*padding: 10px;*/
		box-sizing:border-box;
		background: #10090b;
		opacity: .8;
	    -webkit-transition: all 0.2s ease-in;
	    -moz-transition: all 0.2s ease-in;
	    -ms-transition: all 0.2s ease-in;
	    -o-transition: all 0.2s ease-in;
	    transition: all 0.2s ease-in;
		
	}
	.w-txt>h3{
		position: relative;
		top: -44px;
		/*z-index: 10;*/
		font-family: '微软雅黑';
		font-size: 16px;
		letter-spacing: 1px;
		padding-top: 16px;
		padding-bottom: 12px;
		text-align: center;
		/*background: #10090b;*/
		opacity: .8; 
		color: #fff;
		background: url(./sj.gif);
		background-repeat: repeat-x;
	}
	.w-txt>p{
		line-height: 1.6;
		padding: 0 20px;
	}
	.w-link:hover .w-txt{
		top: 0;
		background: (0,0,0,.8);
	}
	.w-link:hover .w-txt>h3{
		top: 0;
		padding-top: 30px;
	}
	.w-link:hover .wr-img>img{
		-webkit-transform: scale(1.4);
	    -moz-transform: scale(1.4);
	    -ms-transform: scale(1.4);
	    -o-transform: scale(1.4);
	    transform: scale(1.4);
	    -webkit-transition: all 0.2s ease-in;
	    -moz-transition: all 0.2s ease-in;
	    -ms-transition: all 0.2s ease-in;
	    -o-transition: all 0.2s ease-in;
	    transition: all 0.2s ease-in;
	}
</style>
