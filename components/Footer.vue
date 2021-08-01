<template lang="html">
    <footer class="footer">
        <div class="wrapper">
            <div class="nav_container">
                <img src="~/assets/img/header/logo.png" alt="логотип" class="header__logo">
                <nav class="menu">
                    <a 
                    v-for="navitationItem of navigations"
                    :key="navitationItem.href"
                    
                    :href="navitationItem.href" 
                    :class="navitationItem.class">
                        Home
                </a>
                </nav>
            </div>
            <div class="social_network_container social_network_container--footer">
            <DNetwork 
                v-for="networkItem of networks"
                :key="networkItem.link"
                
                :icon="networkItem.icon"
                :link="networkItem.link"
            />
            </div>
        </div>
    </footer>
</template>
<script>
import DNetwork from '~/components/global/Network.vue'
export default {
    components: {
        DNetwork,
    },
    data() {
        return {
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
            ],
            navigations: [
                {
                    href: '#home',
                    class: 'link',
                },
                {
                    href: '#Services',
                    class: 'link',
                },
                {
                    href: '#Extension',
                    class: 'link',
                },
                {
                    href: '#Team',
                    class: 'link',
                },
            ]
        }
    },
}
</script>
<style scoped lang="scss">
.footer {
    height: 150px;
    
    padding-top: 95px;
    
    background-color: #061e37;
}

.nav_container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.link {
    margin-left: 49px;
    
    font-weight: 500;
    font-size: 14px;
    color: #ffffff;

    transition: 0.5s;
}

.link:hover {
    color: #061e37;
}

.social_network_container {
    width: 200px;
   
    margin-top: 30px;
    
    display: flex;
    justify-content: space-between;
}

.social_network_container--footer {
    float: right;
}

@media (max-width: 780px) {
    .footer {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .menu {
        display: none;
    }
}
</style>