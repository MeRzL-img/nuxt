<template lang="html">
    <details class="table services__tables__table">
        <summary class="table__title__container">
            <img class="table__icon" src="~/assets/img/services/1.png" alt="иконка статистики">
            <h3 class="table__title">
                STATISTICS
            </h3>
        </summary>
        <div class="table__footer">
            <img class="table__img" src="~/assets/img/services/01.png" alt="книжка с аайфоном">
            <span class="text__wrapper">
                <p class="text table__text">
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit, 
                    sed do eiusmod tempor incididunt ut labore et dolore magna 
                    aliqua. Ut enim ad minim veniam, 
                </p>        
                <p class="text table__text table__text--down">
                    quis nostrud exercitation 
                    ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis 
                    aute irure dolor in reprehenderit in
                </p>
            </span>
        </div>
    </details>
</template>
<script>
export default {
    
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

.table__footer {
    display: flex;
}

.table__img {
    width: 250;
    
    margin-left: 25px;
    margin-bottom: 25px;
}
</style>