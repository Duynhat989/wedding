<script setup>
import { ref } from 'vue';
import Popup from '../components/Popup.vue'
const showPopup = ref(false)
const showCrun = ()=>{
  showPopup.value = !showPopup.value
}
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
          <div class="time">
            <p>Trân trọng kính mời</p>
            <p>tới tham dự lễ thành hôn của gia đình</p>
            <p class="time_at">Vào lúc:</p>
            <h6>11 giờ 00 phút - Thứ Sáu</h6>
            <p>(Ngày 20 tháng 9 năm Quý Mão)</p>
          </div>
          <div class="address">
            <p class="addesss_at">TƯ GIA NHÀ TRAI:</p>
            <h6>Thôn Thịnh Lương - Xã Thanh Khê</h6>
            <h6>H.Thanh Chương - Nghệ An</h6>
          </div>
          <div class="thank">
            <p>Sự hiện diện của Quý vị là niềm hạnh phúc của gia đình chúng tôi!</p>
          </div>
        </div>
      </div>
    </div>
    <div class="contact">
      <button @click="showCrun" v-if="!showPopup">Gửi mừng cưới</button>
      <button @click="showCrun" v-if="showPopup">Đóng</button>
    </div>
    <Popup v-if="showPopup" />
  </div>
</template>
<style scoped>
.contact{
  position: fixed;
  bottom: 3%;
  width: 100%;
  text-align: center;
}
.contact button{
  border: none;
  background-color: #ff003d;
  color: white;
  padding: 7px 30px;
  border-radius: 6px;
}
.time_at {
  padding-top: 10px;
}

.addesss_at {
  padding: 10px 0;
}

p {
  margin: 0;
  padding: 0;
}

.time {
  margin-top: 20px;
}

.thank p {
  font-size: 0.7em;
  font-style: italic;
}

.time p {
  font-style: italic;
  font-size: 0.9em;
}

.title_pri {
  font-family: 'Times New Roman', Times, serif;
  font-size: 1em;
  font-style: italic;
}

h1 {
  font-family: 'iCiel Monterey Script';
  font-size: 3.5em;
  font-weight: 400;
}

.title_h4 {
  margin-top: 20px;
  font-family: 'Times New Roman', Times, serif;
  font-size: 2em;
  font-style: italic;
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
  height: 90vh;
  width: 100%;
  /* box-shadow: 2px 5px 6px 0px rgba(128, 128, 128, 0.356); */
  padding: 10px;
  position: absolute;
  top: 10%;
}
.background_content {
  border: 1px solid rgba(98, 98, 109, 0.048);
  max-width: 1000px;
  min-height: 200px;
  margin: auto;
  background-color: rgba(255, 255, 255, 0.432);
  border-radius: 10px;
  text-align: center;
  padding-bottom: 30px;
}
/* 
@media only screen and (max-width: 600px) {
  .background_content {
    border: 1px solid rgba(98, 98, 109, 0.048);
    max-width: 1000px;
    height: 90vh;
    margin: auto;
    background-color: rgba(255, 255, 255, 0.432);
    border-radius: 10px;
    text-align: center;
  }
} */


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