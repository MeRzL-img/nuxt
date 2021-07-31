<template lang="html">
    <footer class="footer">
        <div class="wrapper">
            <div class="nav_container">
                <img src="~/assets/img/header/logo.png" alt="логотип" class="header__logo">
                <nav class="menu">
                    <a href="#home" class="link">Home</a>
                    <a href="#Services" class="link">Services</a>
                    <a href="#Extension" class="link">Extension</a>
                    <a href="#Team" class="link">Team</a>
                </nav>
            </div>
            <div class="social_network_container social_network_container--footer">
                <DNetwork 
                icon="../assets/team/01.png"
                link="https://twitter.com/?lang=ru"
            />
            <DNetwork 
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
    }
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
</style>