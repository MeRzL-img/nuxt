<template lang="html">
    <section class="services">
        <DTitle class="services__title">
            Services
        </DTitle>
        <DTxt class="services__text">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
        </DTxt>
        <div class="services__tables">
            <DTable 
                v-for="tableItem of tables"
                :key="tableItem.name"

                :icon="tableItem.icon"
                :name="tableItem.name"
                :image="tableItem.image"
                :text1="tableItem.text1"
                :text2="tableItem.text2"
            />
        </div>
    </section>
</template>
<script>
import DTitle from '~/components/global/Title.vue'
import DTxt from '~/components/global/Text.vue'
import DTable from '~/components/global/Table.vue'
export default {
    components: {
        DTitle,
        DTxt,
        DTable,
    },
    data() {
        return {
            tables: [
                {
                    icon: require('../assets/img/services/1.png'),
                    name: 'SERVICES',
                    image: require('../assets/img/services/01.png'),
                    text1: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,',
                    text2: 'quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in'
                },
                {
                    icon: require('../assets/img/services/2.png'),
                    name: 'INBOX',
                    image: require('../assets/img/services/01.png'),
                    text1: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,',
                    text2: 'quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in'
                },
                {
                    icon: require('../assets/img/services/3.png'),
                    name: 'TEAM',
                    image: require('../assets/img/services/01.png'),
                    text1: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,',
                    text2: 'quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in'
                },
                {
                    icon: require('../assets/img/services/4.png'),
                    name: 'SETTINGS',
                    image: require('../assets/img/services/01.png'),
                    text1: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,',
                    text2: 'quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in'
                },
                {
                    icon: require('../assets/img/services/5.png'),
                    name: 'FEED',
                    image: require('../assets/img/services/01.png'),
                    text1: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,',
                    text2: 'quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in'
                },
            ]
        }
    },
}
</script>
<style scoped lang="scss">
.services {
    max-height: auto;
    
    padding-top: 75px;
    padding-bottom: 20px;

    display: flex;
    flex-direction: column;
    align-items: center;
}

.services__text {
    margin-top: 30px;

    text-align: center;
}

.services__tables {
    margin-top: 50px;
    margin-bottom: 100px;
}

.table__text--down {
    margin-top: 25px;
}

@media (max-width: 980px) {
    .table {
        width: 760px;
    }
}

@media (max-width: 780px) {
    .services {
        height: auto;
    }

    .table {
        width: 300px;
    }

    .table__img {
        display: none;
    }

    .text__wrapper {
        margin-bottom: 10px;
    }

    .services__tables {
        margin-bottom: 10px;
    }
}
</style>
    <!-- <DTable 
        icon="../assets/img/services/2.png"
        name="INBOX"
        image="../assets/img/services/01.png"
        text1="Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,"
        text2="quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in"
    />
    <DTable 
        icon="../assets/img/services/3.png"
        name="TEAM"
        image="../assets/img/services/01.png"
        text1="Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,"
        text2="quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in"
    />
    <DTable 
        icon="../assets/img/services/4.png"
        name="SETTINGS"
        image="../assets/img/services/01.png"
        text1="Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,"
        text2="quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in"
    />
    <DTable 
        class="table__text--down"
        icon="../assets/img/services/5.png"
        name="FEED"
        image="../assets/img/services/01.png"
        text1="Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,"
        text2="quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in"
    /> -->