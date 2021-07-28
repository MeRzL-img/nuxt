<template lang="html">
    <div class="container container--parent">
        <DHeader />
        <main class="main">    
            <div class="wrapper wrapper--main">
                <div class="invitation">
                    <h1 class="main__title">
                        LOREM IPSUM DOLOR SIT AMET
                    </h1>
                    <p class="main__text">
                        Lorem, ipsum dolor sit amet consecteturadipisicing elit. 
                        Voluptatibus consequuntur quae molestiae, aliquam ex 
                        doloremque pariatur repudiandae iusto error quas illum 
                        voluptatum perferendis tempore placea
                    </p>
                    <form action="https://aliexpress.ru/" class="form">
                        <DButton class="main__button main__button--left" />
                        <DButton class="main__button main__button--right" />
                    </form>
                </div>
                <div class="video">
                    <p class="video__text">
                        тут должно быть видео                         
                    </p>
                </div>
            </div>
        </main>
    </div>
</template>
<script>
import DHeader from '~/components/Header.vue'
import DButton from '~/components/global/Button.vue'
export default {
    components: {
        DHeader,
        DButton,
    }    
}
</script>
<style scoped lang="scss">
.container--parent {
    height: 750px;
    
    background-image: url('~/assets/img/backgrounds/bg_header_and_main.jpg');
    background-repeat: no-repeat;
    background-size: cover;
}

.main {
    margin-top: 170px;
}

.wrapper--main {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.invitation {
    display: flex;
    flex-direction: column;
}

.main__title {
    max-width: 420px;
    
    color: #ffffff;
    font-size: 40px;
    font-weight: 900;
}

.main__text {
    max-width: 530px;

    margin-bottom: 38px;

    font-size: 18px;
    color: #ffffff;
}

.form {
    max-width: 340px;
    
    display: flex;
    justify-content: space-between;
}

.main__button {
    height: 55px;

    border-radius: 5%;
    border: none;

    font-size: 14px;

    transition: 0.4s;
}

.main__button:hover {
    box-shadow: 0.4em 0.4em 5px rgba(122,122,122,0.5);
    cursor: pointer
}

.main__button--left {
    width: 150px;
    
    color: #eef0f2;

    background: #061e37;
}

.main__button--right {
    width: 160px;
    
    color: #061e37;
    font-weight: bold;

    background: #ffffff;
}

.video {
    width: 600px;
    height: 300px;

    border: 1px solid;
    border-color: #000000;
    border-radius: 1%;
    
    display: flex;
    justify-content: center;
    align-items: center;

    background: #ffffff;
}
</style>