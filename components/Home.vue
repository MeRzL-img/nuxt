<template lang="html">
    <section class="home">
        <div class="wrapper wrapper--home">
            <DTitle />
            <h3 class="home__subtitle">
                Project Managment Tool
            </h3>
            <DTxt class="home__text" />
            <div class="wrapper--row">
                <DProfession />
                <DProfession />
                <DProfession />
            </div>
            <DButton class="home__button" />
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
    }
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
    width: 150px;
    height: 55px;
    
    border-radius: 5%;
    border: none;
    
    font-size: 11px;
    font-weight: bold;
    color: #ffffff;

    background: #1de9b6;

    transition: 0.5s;
}
</style>