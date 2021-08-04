<template lang="html">
    <section class="extension">
        <div class="wrapper wrapper--extension">
            <div class="extension__container extension__container--left">
                <DTitle class="extension__title">
                    What our customers have to say about us.
                </DTitle>
                <DTxt class="extension__text">
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
                </DTxt>
                <form class="extension__form" action="http://snake.io/">
                    <DButton class="extension__form__button">
                        GET STARTED
                    </DButton>
                    <!-- <v-btn
                        class="extension__form__button"
                        elevation="2"
                        x-large
                        color="#061e37"
                        min-height="55px"
                    >
                        GET STARTED
                    </v-btn> -->
                </form>
            </div>
            <div class="extension__container extension__container--right">
                <DName 
                    v-for="nameTableItem of nameTables"
                    :key="nameTableItem.name"
                    
                    :name="nameTableItem.name" 
                    :text="nameTableItem.text"
                    :avatar="nameTableItem.avatar"
                    :class="nameTableItem.class"
                />
            </div>
        </div>
    </section>
</template>
<script>
import DTitle from '~/components/global/Title.vue'
import DTxt from '~/components/global/Text.vue'
import DButton from '~/components/global/Button.vue'
import DName from '~/components/global/NameTable.vue'
export default {
    components: {
        DTitle,
        DTxt,
        DButton,
        DName,
    },
    data() {
        return {
            nameTables: [
                {
                    name: 'Jhon Doe',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea',
                    avatar: require('../assets/img/extension/1.png')
                },
                {
                    name: 'Khalessi',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea',
                    avatar: require('../assets/img/extension/2.png'),
                    class: 'extension__name_tables_container--down'
                },
            ]
        }
    }
}
</script>
<style scoped lang="scss">
.extension {
    width: 100%;
    height: 565px;

    padding-top: 87px;
    
    background-image: url("~/assets/img/backgrounds/bg_extension.jpg");
    background-repeat: no-repeat;
    background-size: cover;
}

.wrapper--extension {
    display: flex;
    justify-content: space-between;
}

.extension__title {
    width: 440px;

    font-size: 44px;
    color: #ffffff;
    font-weight: 500;
}

.extension__text {
    width: 514px;

    margin-top: 30px;
    
    font-size: 14px;
    color: #ffffff;
}

.extension__container--left {
    margin-top: 50px;
}

.extension__form {
    ::v-deep {
        .extension__form__button{
            width: 150px;
            padding: 0;
            height: 55px;
            font-size: 15px;
            background: #061e37;
        }
    }
}

.extension__form__button {
    max-width: 150px;
    height: 55px;

    margin-top: 80px;
    
    border-radius: 5%;
    border: none;
    
    font-size: 15px;
    font-weight: bold;
    color: #ffffff;

    background: #061e37;

    transition: 0.5s;
}

.extension__form__button:hover {
    box-shadow: 0.4em 0.4em 5px rgba(122,122,122,0.5);
    cursor: pointer
}

.extension__name_tables_container--down {
    margin-top: 70px;
}

@media (max-width: 1170px) {
    .extension {
        height: auto;

        padding-bottom: 10px;
    }

    .wrapper--extension {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
    }

    .extension__container--right {
        margin-top: 40px;
    }

    .name_tables_container__name_table {
        text-align: start;
    }
}

@media (max-width: 980px) {
    .extension__text {
        text-align: center;
    }
}

@media (max-width: 780px) {
    .extension__container--right {
        display: none;
    }

    .extension__title {
        width: auto;
        max-width: 460px;
    }

    .extension__text {
        width: auto;
        max-width: 460px;
    }

}
</style>
    <!-- <DName 
        name="Khalessi" 
        text="Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea" 
        avatar="../assets/img/extension/2.png"
        class="extension__name_tables_container--down"
    /> -->