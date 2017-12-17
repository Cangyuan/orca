<template>
	<div class="me-info">
		<div class="me">
			<span class="close" @click="closeMe">&times</span>
			<div class="me-pic">
				<div class="me-wrap">
					<img src="./me-open.jpg" alt="">
				</div>			
			</div>		
			<h3>orca</h3>
			<p class="me-txt">目前从事界面设计、交互设计、用户体验、前端开发及网页重构等相关工作~</p>
			<p class="detail de-close"><a href="#about" @click="closeMe">个人详情...</a></p>
			<p class="detail"><a href="file/resume.pdf" class="download">简历pdf</a></p>
		</div>
	</div>
</template>
<script>
export default {
  name: 'me',
  data () {
    return {
      //msg: 'header part'
    }
  },
  methods:{
  	closeMe:function(){
      $('.me-info').removeClass('open-me');
      $('.wrap').removeClass('remove');
      $('.main-bg').css('display', 'none');
    }
  }
}
</script>
<style>

</style>