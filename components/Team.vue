<template lang="html">
    <section class="team">
        <DTitle class="team__title">
            Our Team
        </DTitle>
        <DTxt class="team__text team__text--top">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
        </DTxt>
        <div class="team__avatar_container avatar_container">
            <DAvatar 
                v-for="avatarItem of avatars"
                :key="avatarItem.avatar"

                :avatar="avatarItem.avatar"
            />
        </div>
        <DTxt class="team__text team__text--bottom">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magnaLorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt
        </DTxt>    
        <div class="social_network_container">
            <DNetwork 
                v-for="networkItem of networks"
                :key="networkItem.link"
                
                :icon="networkItem.icon"
                :link="networkItem.link"
            />
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
    },
    data() {
        return {
            avatars: [
                {
                    avatar: require('../assets/img/team/1.jpg')
                },
                {
                    avatar: require('../assets/img/team/2.jpg')
                },
                {
                    avatar: require('../assets/img/team/3.jpg')
                },
            ],
            networks: [
                {
                    icon: require('../assets/img/team/01.png'),
                    link: 'https://twitter.com/?lang=ru'
                },
                {
                    icon: require('../assets/img/team/02.png'),
                    link: 'https://ru-ru.facebook.com/'
                },
                {
                    icon: require('../assets/img/team/03.png'),
                    link: 'https://www.linkedin.com/'
                },
                {
                    icon: require('../assets/img/team/04.png'),
                    link: 'https://www.nba.com/bulls/'
                },
                {
                    icon: require('../assets/img/team/05.png'),
                    link: 'https://www.behance.net/'
                },
            ]
        }
    },
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

@media (max-width: 780px) {
    .team__avatar_container {
        margin: 50px 0;
        width: auto;

        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .team__text {
        width: auto;
        max-width: 460px;
    }

    .team {
        padding-bottom: 20px;
    }
}
</style>
    <!-- <DAvatar 
        avatar="../assets/img/team/2.jpg"
    />
    <DAvatar 
        avatar="../assets/img/team/3.jpg"
    /> -->
    <!-- <DNetwork 
        icon="../assets/team/02.png"
        link="https://ru-ru.facebook.com/"
    />
    <DNetwork 
        icon="../assets/team/03.png"
        link="https://www.linkedin.com/"
    />
    <DNetwork 
        icon="../assets/team/04.png"
        link="https://www.nba.com/bulls/"
    />
    <DNetwork 
        icon="../assets/team/05.png"
        link="https://www.behance.net/"
    /> -->