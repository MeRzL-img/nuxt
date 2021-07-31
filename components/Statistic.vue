<template lang="html">
    <section class="ads">
        <DStats
            class="ads__container--cyan" 
            icon="../assets/img/ads/01.png"
            number="12000+"
            text="Business"
        />
        <DStats 
            class="ads__container--blue" 
            icon="../assets/img/ads/02.png"
            number="60000+"
            text="Downloads"
        />
        <DStats 
            class="ads__container--purple" 
            icon="../assets/img/ads/03.png"
            number="30000+"
            text="Free Installs"
        />
        <DStats 
            class="ads__container--pink" 
            icon="../assets/img/ads/04.png"
            number="40000+"
            text="Pro Users"
        />
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