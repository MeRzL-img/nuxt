<template lang="html">
    <div>
        <DMain />
        <DHome />
        <DAdvertising />
        <DServices />
        <DExtension />
        <DTeam />
        <DFooter />
    </div>
</template>
<script>
import DMain from '~/components/Main.vue'
import DHome from '~/components/Home.vue'
import DAdvertising from '~/components/Statistic.vue'
import DServices from '~/components/Services.vue'
import DExtension from '~/components/Extension.vue'
import DTeam from '~/components/Team.vue'
import DFooter from '~/components/Footer.vue'
export default {
    components: {
        DMain,
        DHome,
        DAdvertising,
        DServices,
        DExtension,
        DTeam,
        DFooter,
    }
}
</script>
<style lang="scss">
* {
    padding: 0;
    margin: 0;
}

html {
    scroll-behavior: smooth;
}

body {
    width: 100%;
    
    font-family: 'Raleway', sans-serif;
}

a {
    text-decoration: none;
}
.wrapper {
    max-width: 1170px;
    margin: 0px auto;
    padding: 0px 15px;
}


@media (max-width: 1170px) {
    .wrapper {
        max-width: 960px;
    }
}

@media (max-width: 980px) {
    .wrapper {
        max-width: 768px;
    }
}

@media (max-width: 780px) {
    .wrapper {
        max-width: none;
        
        display: flex;
        flex-direction: column;    
    }
}
</style>