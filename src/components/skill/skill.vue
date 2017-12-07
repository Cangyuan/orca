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
      msg: 'header part'
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
</style>