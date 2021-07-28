<template lang="html">
    <div class="ads__container">
        <img class="ads__container__img" src="~/assets/img/ads/01.png" alt="фото зданий">
        <div class="ads__container__text-wrapper">
            <p class="ads__container__text">
                12000+
            </p>
            <p class="ads__container__text">
                Business
            </p>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped lang="scss">
.ads__container {
    height: 150px;
    width: 25%;

    display: flex;
    justify-content: center;
    align-items: center;
}

.ads__container__img {
    width: 60px;
    height: 60px;
}

.ads__container__text {
    margin-left: 24px;
    
    font-size: 15px;
    color: #ffffff;
    font-weight: bold;
}
</style>