<template lang="html">
    <section class="home">
        <div class="wrapper wrapper--home">
            <DTitle>
                Easy & Useful
            </DTitle>
            <h3 class="home__subtitle">
                Project Managment Tool
            </h3>
            <DTxt class="home__text">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Ad laboriosam dolores labore provident possimus? Tempora incidunt obcaecati, excepturi dicta ratione nisi totam
            </DTxt>
            <div class="wrapper--row">
                <DProfession
                    v-for="professionItem of professions"
                    :key="professionItem.avatar"

                    :avatar="professionItem.avatar"
                    :title="professionItem.title"
                    :text="professionItem.text"
                />
            </div>
            <v-btn
                class="home__button"
                elevation="2"
                x-large
                color="#1de9b6"
                min-height="55px"
            >
                GET STARTED
            </v-btn>
            
            <!-- <DButton class="home__button">
                GET STARTED
            </DButton> -->
        </div>    
    </section>    
</template>
<script>
import DTitle from '~/components/global/Title.vue'
import DTxt from '~/components/global/Text.vue'
import DProfession from '~/components/global/Profession.vue'
import DButton from '~/components/global/Button.vue'
export default {
    components: {
        DTitle,
        DTxt,
        DProfession,
        DButton,
    },
    data() {
        return {
            professions: [
                {
                    avatar: require('../assets/img/home/calendar.png'),
                    title: 'Title Goes Here',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Minus nulla vitae numquam perspiciatis quod! Sequi modi magnam unde delectus nulla, quia'
                },
                {
                    avatar: require('../assets/img/home/human.png'),
                    title: 'Title Goes Here',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Minus nulla vitae numquam perspiciatis quod! Sequi modi magnam unde delectus nulla, quia'
                },
                {
                    avatar: require('../assets/img/home/working.png'),
                    title: 'Title Goes Here',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Minus nulla vitae numquam perspiciatis quod! Sequi modi magnam unde delectus nulla, quia'
                },
            ]
        }
    },
}
</script>
<style scoped lang="scss">
.home {
    height: 600px;
    
    padding-top: 75px;
}

.wrapper--home {
    display: flex;
    flex-direction: column;
    align-items: center;   
}

.home__subtitle {
    margin-top: 15px;
    
    font-size: 19px;
    color: #b0bec5;
}

.home__text {
    margin-top: 22px;

    text-align: center;
}

.wrapper--row {
    width: 100%;

    margin-top: 98px;
    margin-bottom: 78px;
    
    display: flex;
    justify-content: space-between;
}

.home__button {
    max-width: 150px;
    height: 55px;
    
    border-radius: 5%;
    border: none;
    
    font-size: 11px;
    font-weight: bold;
    color: #ffffff;

    background: #1de9b6;

    transition: 0.5s;
}

@media (max-width: 980px) {
    .home {
        height: 1040px;
    }

    .wrapper--row {
        height: 650px;
        
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
    }
}
</style>
    <!-- <DProfession
        avatar="../assets/img/home/human.png"
        title="Title Goes Here"
        text="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Minus nulla vitae numquam perspiciatis quod! Sequi modi magnam unde delectus nulla, quia"
    />
    <DProfession
        avatar="../assets/img/home/working.png"
        title="Title Goes Here"
        text="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Minus nulla vitae numquam perspiciatis quod! Sequi modi magnam unde delectus nulla, quia"
    /> -->