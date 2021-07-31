<template lang="html">
    <div class="ads__container">
        <img class="ads__container__img" :src="(icon)" alt="фото зданий">
        <div class="ads__container__text-wrapper">
            <p class="ads__container__text">
                {{ number }}
            </p>
            <p class="ads__container__text">
                {{ text }}
            </p>
        </div>
    </div>
</template>
<script>
export default {
    props: {
        icon: {
            type: String,
            default: '',
        },
        number: {
            type: Number,
            default: '',
        },
        text: {
            type: String,
            default: '',
        },
    },
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