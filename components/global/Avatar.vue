<template lang="html">
    <img :src="(avatar)" alt="фото человека" class="avatar_container__avatar">
</template>
<script>
export default {
    props: {
        avatar: {
            type: String,
            default: '',
        },
    },
}
</script>
<style scoped lang="scss">
.avatar_container__avatar {
    width: 100px;
    height: 100px;

    opacity: 0.3;

    border-radius: 50%;

    transition: 0.5s;
}

.avatar_container__avatar:hover {
    transform: scale(1.3);
    opacity: 1;

    box-shadow: 0 0 10px rgba(0,0,0,1.2);
}
</style>