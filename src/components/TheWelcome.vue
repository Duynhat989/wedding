<script setup>

</script>

<template>
  <div class="container-fluid">
    <div class="header_content">
      <i class='bx bxs-heart'></i>&emsp;Happy wedding&emsp;<i class='bx bxs-heart'></i>
    </div>
    <div class="content">
      <div class="banner">
        <div class="d">
          <div class="banner_content">
            <img src="../assets/images/w4.jpg" alt="">
          </div>
        </div>
      </div>
      <div class="background">
        <div class="background_content">
          <div class="title">
            <h4 class="title_h4">Thư mời</h4>
          </div>
          <div class="title">
            <h4 class="title_pri">Đến tham dự lễ thành hôn</h4>
          </div>
          <div class="chapter">
            <div class="row">
                <div class="col-5">
                  <h1>Thành Vinh</h1>
                </div>
                <div class="col-2">
                  <h1>&</h1>
                </div>
                <div class="col-5">
                  <h1>Như Quỳnh</h1>
                </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.title_pri{
  font-family:'Times New Roman', Times, serif;
  font-size: 1em;
  font-style: italic;
}
h1{
  font-family: 'iCiel Monterey Script';
  font-size: 3.5em;
  font-weight: 400;
}
.title_h4{
  font-family: 'iCiel Monterey Script';
  font-size: 4em;
}
.banner {
  width: 100%;
  opacity: 0.4;
}

.banner_content {
  width: 100%;
}

.banner_content img {
  width: 100%;
  height: 100vh;
  object-fit: cover;
}

.container-fluid {
  padding: 0;
}

.background {
  height: 80vh;
  width: 100%;
  /* box-shadow: 2px 5px 6px 0px rgba(128, 128, 128, 0.356); */
  padding: 10px;
  position: absolute;
  top: 7%;
}

.background_content {
  border: 1px solid rgba(98, 98, 109, 0.048);
  max-width: 1000px;
  height: 80vh;
  margin: auto;
  background-color: rgba(255, 255, 255, 0.432);
  border-radius: 10px;
  text-align: center;
}

.background_content img {
  object-fit: cover;
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  transform: skewY(100px)
    /* transform: translate(-50%, -50%); */
}

.view {
  position: absolute;
  top: 0;
}

.content {
  padding: 0px;
  position: relative;
  min-height: 100vh;
  background-color: rgba(255, 238, 214, 0.137);
}

.header_content {
  height: 50px;
  line-height: 50px;
  text-align: center;
  position: fixed;
  top: 0;
  z-index: 999;
  width: 100%;
  font-size: 30px;
  font-family: 'iCiel Monterey Script';
}

.backgroud img {
  object-fit: cover;
  width: 100%;
}

.img img {
  width: 100%;
}

.right {
  padding: 20px;
}

.left {
  padding: 20px;
}

img {
  object-fit: contain;
  /* height: 1000px; */
}

.right_content {
  /* width: 500px; */
  /* margin: auto; */
}

.left_content {
  /* width: 500px; */
  /* margin: auto */
}</style>