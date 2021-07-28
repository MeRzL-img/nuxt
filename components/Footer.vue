<template lang="html">
    <footer class="footer">
        <div class="wrapper">
            <div class="nav_container">
                <img src="~/assets/img/header/logo.png" alt="логотип" class="header__logo">
                <nav class="menu">
                    <a v-for="i of 5" :key="i" href="#home" class="link">Home</a>
                </nav>
            </div>
            <div class="social_network_container social_network_container--footer">
                <DNetwork />
                <DNetwork />
                <DNetwork />
                <DNetwork />
                <DNetwork />
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