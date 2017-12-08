<template>
  <footer>
    <div class="wrap-bottom">
      <p>copyright © by orca</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'footer',
  data () {
    return {
      //msg: 'header part'
    }
  }
}
</script>
<style>

footer{
  background: #333;
  color: #fff;
  padding: 20px 0;
  text-align: center;
  letter-spacing: 1px;
}
.wrap-bottom p{
  padding: 15px 0;
}
</style>