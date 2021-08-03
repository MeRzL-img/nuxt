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
                        <v-btn
                            class="main__button main__button--left"
                            elevation="2"
                            x-large
                            color="#061e37"
                            min-height="55px"
                        >
                            BUY NOW
                        </v-btn>
                        <v-btn
                            class="main__button main__button--right"
                            elevation="2"
                            x-large
                            color="#ffffff"
                            min-height="55px"
                        >
                            TRY FOR FREE
                        </v-btn>
                        <!-- <DButton class="main__button main__button--left">
                            BUY NOW
                        </DButton> -->

                        <!-- <DButton class="main__button main__button--right">
                            TRY FOR FREE
                        </DButton> -->
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
    max-width: 100%;
    
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
    
    border: none;

    font-size: 14px;

    transition: 0.4s;
    z-index: 10;
}

// .main__button:hover {
//     box-shadow: 0.4em 0.4em 5px rgba(122,122,122,0.5);
//     cursor: pointer
// }

.main__button--left {
    max-width: 150px;
    
    color: #ffffff;

    background-color: #061e37;
}

.main__button--right {
    max-width: 160px;
    height: 55px;
    
    color: #061e37;
    font-weight: bold;

    background-color: #ffffff;
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


@media (max-width: 1170px) {
.video {
        width: 500px;
        height: 250px;
    }
}

@media (max-width: 980px) {
    .video {
        width: 400px;
        height: 200px;
    }
}

@media (max-width: 780px) {
    .container--parent {
        height: 1000px;
        
        background-size: auto 1000px;
    }

    .main {
        display: flex;
        flex-direction: column;
        align-items: center;

    }

    .invitation {
        display: flex;
        flex-direction: column;
        align-items: center;
        
        text-align: center;
    }

    .main__button {
        width: 130px;
    }
    
    .wrapper--header {
        display: flex;
        flex-direction: row;
    }

    .menu {
        display: none;
    }

    .main__button--left {
        margin-right: 20px;
    }

    .video {
        width: 280px;
        height: 140px;

        margin-top: 50px;
    }  
}
</style>