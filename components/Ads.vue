<template lang="html">
    <section class="ads">
        <DStats class="ads__container--cyan" />
        <DStats class="ads__container--blue" />
        <DStats class="ads__container--purple" />
        <DStats class="ads__container--pink" />
    </section>
</template>
<script>
import DStats from '~/components/global/Stats.vue'
export default {
    components: {
        DStats,
    }
}
</script>
<style scoped lang="scss">
.ads {
    width: 100%;
    height: 150px;

    display: flex;
}

.ads__container--cyan {
    background: #80d8ff;
}

.ads__container--blue {
    background: #82b1ff;
}

.ads__container--purple {
    background: #b388ff;
}

.ads__container--pink {
    background: #ea80fc;
}
</style>