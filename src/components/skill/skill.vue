<template>
  <section id="skill">
	  <div class="wrap-sk">
	    <div class="se-title sk-skill">
	      <h2>技能</h2>
	      <span class="border"></span>
	      <h4>my skills</h4>
	    </div>
	    <div class="sk-content">
	      <ul>
	        <li>
	          <div class="sk-co-title">
	            <h4>编程</h4>
	            <p>Programming Skills</p>
	          </div>
	          <ul class="sk-list">
	            <li>html,html5</li>
	            <li>css,css3</li>
	            <li>javascript</li>
	            <li>nodejs</li>
	            <li>mongodb</li>
	          </ul>
	        </li>
	        <li>
	          <div class="sk-co-title">
	            <h4>框架</h4>
	            <p>Frame Skills</p>
	          </div>
	          <ul class="sk-list">
	            <li>bootstrap</li>
	            <li>jquery</li>
	            <li>angularjs</li>
	            <li>express</li>
	          </ul>
	        </li>
	        <li>
	          <div class="sk-co-title">
	            <h4>编辑器</h4>
	            <p>Editor Skills</p>
	          </div>
	          <ul class="sk-list">
	            <li>sublime</li>
	            <li>webstrom</li>
	            <li>eclipse</li>
	            <li>notepad++</li>
	          </ul>
	        </li>
	        <li>
	          <div class="sk-co-title">
	            <h4>设计</h4>
	            <p>Design Skills</p>
	          </div>
	          <ul class="sk-list">
	            <li>adobe photoshop</li>
	            <li>adobe illustrator</li>
	            <li>axure rp</li>
	          </ul>
	        </li>
	      </ul>
	    </div>
	  </div>
	</section>
</template>

<script>
export default {
  name: 'skill',
  data () {
    return {
      // msg: 'header part'
    }
  }
}
</script>
<style>
 #skill{
  position: relative;
  background: url(./skill-bg.jpg);
  background-attachment: fixed;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
 }
 #skill:after{
  position: absolute;
  top: 0;
  left: 0;
  content: '';
  display: block;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,.4);
 } 
 .sk-skill{
 	color: #fff;
 }
 .wrap-sk{
 	position: relative;
 	z-index: 4;
 }
 .sk-content{
 	color: #fff;
 	padding: 0 20px;
 	margin-top: 15px;
 }
 .sk-content>ul{
 	display: table;
 	width: 100%;
 }
 .sk-content>ul>li{
 	display: table-cell;
 	width: 25%;
 	text-align: center;
 }
 .sk-co-title>p{
 	font-style: italic;
 	color: #ccc;
 	margin: 10px 0 20px 0;
 }
 .sk-list{
 	width: 100%;
 }
 .sk-list>li{
 	width: 90%;
 	padding: 15px 0;
 	margin: 15px auto;
 	border:1px solid #fff;
 	text-transform: uppercase;
 	letter-spacing: 2px;
 	font-size: 16px;
 }
</style>