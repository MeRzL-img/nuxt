<template lang="html">
    <div class="column">
        <img class="column__icon" src="~/assets/img/home/calendar.png" alt="иконка календаря">
        <h2 class="column__title">Title Goes Here</h2>
        <p class="column__text">
            Lorem ipsum dolor sit amet, consectetur 
            adipisicing elit. Minus nulla vitae numquam 
            perspiciatis quod! Sequi modi magnam unde 
            delectus nulla, quia
        </p>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped lang="scss">
.column {
    max-width: 300px;

    display: flex;
    flex-direction: column;
    align-items: center;
}

.column__title {
    margin-top: 44px;
    
    font-size: 15px;
    color: #061e37;
}

.column__text {
    margin-top: 20px;
    
    text-align: center;
    
    font-size: 11px;
    color: #78909c;
}
</style>