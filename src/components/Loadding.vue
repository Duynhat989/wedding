<style scoped>
.loadding {
    color: rgb(75, 75, 75);
    min-height: 90vh;
    /* background-color: black; */
    position: relative;
    width: 100%;
}

.loadding_content {
    position: absolute;
    top: 50%;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
}

.loader {
    position: relative;
    width: 40px;
    height: 60px;
    animation: heartBeat 1.2s infinite cubic-bezier(0.215, 0.61, 0.355, 1);
}

.loader:before,
.loader:after {
    content: "";
    background: #ff3d00;
    width: 40px;
    height: 60px;
    border-radius: 50px 50px 0 0;
    position: absolute;
    left: 0;
    bottom: 0;
    transform: rotate(45deg);
    transform-origin: 50% 68%;
    box-shadow: 5px 4px 5px #0004 inset;
}

.loader:after {
    transform: rotate(-45deg);
}

@keyframes heartBeat {
    0% {
        transform: scale(0.95)
    }

    5% {
        transform: scale(1.1)
    }

    39% {
        transform: scale(0.85)
    }

    45% {
        transform: scale(1)
    }

    60% {
        transform: scale(0.95)
    }

    100% {
        transform: scale(0.9)
    }
}

.title {
    padding: 30px 15px;
    font-family: 'iCiel Monterey Script';
    font-size: 1.7em;
    font-weight: 900;
}

.loadding_title {
    position: absolute;
    top: 0%;
    width: 100%;
    display: flex;
}

.view-title {
    width: 100%;
    text-align: center;
    align-items: center;
    justify-content: center;
    display: flex;
}
.img-loadding{
    object-fit: cover;
    width: 100%;
    height: 100vh;
    opacity: 0.3;
}
</style>
<template>
    <div class="loadding">
        <img src="../assets/images/w2.jpg" class="img-loadding">
        <div class="loadding_title">
            <div class="view-title">
                <span class="title">Thành Vinh</span><i class='bx bx-heart'></i><span class="title">Như Quỳnh</span>
            </div>
        </div>
        <div class="loadding_content">
            <span class="loader"></span>
        </div>
    </div>
</template>
<script setup>

</script>