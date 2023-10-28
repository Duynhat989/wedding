<style scoped>
.popup{
    position: fixed;
    top: 15%;
    width: 100%;
    text-align: center;
}
.popup_content{
    width: 350px;
    margin: auto;
    min-height: 500px;
    background-color: aliceblue;
    padding: 15px;
}
.top{
    padding: 5px;
}
.popup_content .top img{
    width: 100%;

}
h5{
    font-style: italic;

}
.bank{
    margin-top: 10px;
}
.bank h6{
    font-style: italic;
    font-size: 15px;
    padding: 0;
    margin: 0;
}
.title p{
    font-style: italic;
    font-size: 13px;
    padding: 0;
    margin: 0;
}
</style>
<template>
    <div class="popup">
        <div class="popup_content">
            <div class="title">
                <h5>Xin chân thành cảm ơn</h5>
            </div>
            <div class="top">
                <img :src="url" alt="">
            </div>
            <div class="bank">
                <h6>Tên người nhận: {{ name }}</h6>
                <h6>Số tài khoản: 109868930749</h6>
                <h6>Ngân hàng: {{ bank }}</h6>
            </div>
            <div class="title">
                <p>Vui lòng ghi nội dung là người gửi</p>
                <p>để chúng tôi có thể gửi lời cảm ơn đến bạn!</p>
            </div>
        </div>
    </div>
</template>
<script setup>
import { ref } from 'vue';

const stk = ref("109868930749")
const bank = ref("vietinbank")
const name = ref("Nguyen Thanh Vinh")
const url = ref(`https://img.vietqr.io/image/${bank.value}-${stk.value}-compact.jpg?amount=0&addInfo=Happy Wedding`)
</script>