<template lang="html">
    <div class="column">
        <img class="column__icon" :src="(avatar)" alt="иконка">
        <h2 class="column__title">{{ title }}</h2>
        <p class="column__text">
            {{ text }}
        </p>
    </div>
</template>
<script>
export default {
    props: {
        avatar: {
            type: String,
            default: '',
        },
        title: {
            title: String,
            default: '',
        },
        text: {
            text: String,
            default: '',
        },
    },
}
</script>
<style scoped lang="scss">
.column {
    max-width: 300px;

    display: flex;
    flex-direction: column;
    align-items: center;
}

.column__title {
    margin-top: 44px;
    
    font-size: 15px;
    color: #061e37;
}

.column__text {
    margin-top: 20px;
    
    text-align: center;
    
    font-size: 11px;
    color: #78909c;
}
</style>