<template lang="html">
    <details class="table services__tables__table">
        <summary class="table__title__container">
            <img class="table__icon" :src="(icon)" alt="иконка">
            <h3 class="table__title">
                {{ name }}
            </h3>
        </summary>
        <div class="table__footer">
            <img class="table__img" :src="(image)" alt="книжка с аайфоном">
            <span class="text__wrapper">
                <p class="text table__text">
                    {{ text1 }} 
                </p>        
                <p class="text table__text table__text--down">
                    {{ text2 }}
                </p>
            </span>
        </div>
    </details>
</template>
<script>
export default {
    props: {
        icon: {
            type: String,
            default: '',
        },
        name: {
            type: String,
            default: '',
        },
        image: {
            type: String,
            default: '',
        },
        text1: {
            type: String,
            default: '',
        },
        text2: {
            type: String,
            default: '',
        },

    },
}
</script>
<style scoped lang="scss">
.table {
    width: 800px;

    margin-top: 20px;

    box-shadow: 0 0 7px rgba(0, 0, 0, 0.2);

    border-radius: 10px;
}

.table__title__container {
    height: 50px;
    
    display: flex;
    align-items: center;
}

.table__title__container:hover {
    cursor: pointer
}

.table__title__container :-webkit-details-marker {
    display: none;
}

.table__icon {
    width: 18px;
    
    margin-left: 20px;
}

.table__title {
    margin-left: 30px;

    font-size: 17px;
}

.table__text {
    max-width: none;

    padding: 0px 25px;
    
    color: #000000;
    font-weight: bold;
    font-size: 15px;
    
    text-align: start;
}

.table__text--down {
    margin-top: 20px;
}

.table__footer {
    display: flex;
}

.table__img {
    width: 250;
    
    margin-left: 25px;
    margin-bottom: 25px;
}

@media (max-width: 780px) {
    .table__img {
        display: none;
    }
}
</style>