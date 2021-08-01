<template lang="html">
    <header class="header">
        <div class="wrapper wrapper--header">
            <img src="~/assets/img/header/logo.png" alt="логотип" class="header__logo">
            <nav class="menu">
                <a 
                    v-for="navitationItem of navigations"
                    :key="navitationItem.href"
                    
                    :href="navitationItem.href" 
                    :class="navitationItem.class">
                        Home
                </a>
                <!-- <a href="#Services" class="link">Services</a>
                <a href="#Extension" class="link">Extension</a>
                <a href="#Team" class="link">Team</a> -->
            </nav>
            <form action="https://accounts.google.com/signup/v2/webcreateaccount?hl=en&flowName=GlifWebSignIn&flowEntry=SignUp">
                <button class="header__button" href="">
                    sign up
                </button>
            </form>
        </div>
    </header>
</template>
<script>
export default {
    data() {
        return {
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
.header {
    padding-top: 52px;
}

.wrapper--header {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.header__logo {
    width: 180px;
}

.link {
    margin-right: 49px;
    
    font-weight: 500;
    font-size: 14px;
    color: #ffffff;

    transition: 0.5s;
}

.link:hover {
    color: #061e37;
}

.link--last {
    margin-right: 0px;
}

.header__button {
    width: 80px;
    height: 25px;

    font-size: 14px;
    color: #ffffff;

    border-radius: 5%;
    border: 1px solid;
    border-color: #ffffff;
    border-style: solid;
    
    background: Transparent;

    transition: 0.4s;
}

.header__button:hover {
    transform: scale(1.2);
    cursor: pointer
}

@media (max-width: 780px) {
    .wrapper--header {
        display: flex;
        flex-direction: row;
    }

    .menu {
        display: none;
    }
}
</style>