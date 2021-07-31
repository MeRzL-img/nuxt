<template lang="html">
   <a :href="(link)"><img :src="(icon)" alt="icon" class="social_network"></a>
</template>
<script>
export default {
    props: {
        icon: {
            type: String,
            default: '',
        },
        link: {
            type: String,
            default: '',
        },
    },
}
</script>
<style scoped lang="scss">
.social_network {
    height: 18px;
}
</style>