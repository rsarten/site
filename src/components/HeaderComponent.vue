<template>
  <div class="banner">
    <div class="banner-block">
      <h1>rorysarten.co.nz</h1>
      <p>I am Rory Sarten.  This is my project server where I test ideas, run web-crawlers and host applications.</p>
    </div>
    <div class="banner-block">
      <img alt="Vue logo" src="../assets/networking-538.png" style="width:300px;height:150px">
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderComponent'
}
</script>

<style scoped>

div.banner {
  width: 70%;
  margin: 10px auto;
  position: relative;
  text-align:center;
}

div.banner_block {
  width: 300px;
  display:inline-block;
  margin: 10px;
  text-align:right
}

</style>