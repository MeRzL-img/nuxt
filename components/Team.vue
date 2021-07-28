<template lang="html">
    <section class="team">
        <DTitle class="team__title" />
        <DTxt class="team__text team__text--top" />
        <div class="team__avatar_container avatar_container">
            <DAvatar />
            <DAvatar />
            <DAvatar />
        </div>
        <DTxt class="team__text team__text--bottom" />
        <div class="social_network_container">
            <DNetwork />
            <DNetwork />
            <DNetwork />
            <DNetwork />
            <DNetwork />
        </div>
    </section>
</template>
<script>
import DTitle from '~/components/global/Title.vue'
import DTxt from '~/components/global/Text.vue'
import DAvatar from '~/components/global/Avatar.vue'
import DNetwork from '~/components/global/Network.vue'
export default {
    components: {
        DTitle,
        DTxt,
        DAvatar,
        DNetwork,
    }
}
</script>
<style scoped lang="scss">
.team {
    height: 650px;
    
    padding-top: 75px;

    display: flex;
    flex-direction: column;
    align-items: center;

    text-align: center;
}

.team__text--top {
    margin-top: 30px;
}

.team__avatar_container {
    width: 460px;
    height: 360px;

    display: flex;
    justify-content: space-between;
    align-items: center;
}

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

.social_network_container {
    width: 200px;
   
    margin-top: 30px;
    
    display: flex;
    justify-content: space-between;
}
</style>