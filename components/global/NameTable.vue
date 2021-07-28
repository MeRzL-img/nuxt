<template lang="html">
    <div class="extension__name_tables_container name_tables_container">
        <img src="~/assets/img/extension/1.png" alt="фото парня" class="avatar">
        <div class="name_tables_container__name_table">
            <h3 class="name_table__name">
                John Doe
            </h3>
            <p class="name_table__description">
                Lorem ipsum dolor sit amet, consectetur 
                adipisicing elit, sed do eiusmod tempor 
                incididunt ut labore et dolore magna 
                aliqua. Ut enim ad minim veniam, quis 
                nostrud exercitation ullamco laboris 
                nisi ut aliquip ex ea
            </p>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped lang="scss">
.name_tables_container__name_table {
    width: 450px;
    height: 160px;

    margin-left: 50px;
    padding-left: 30px;

    display: flex;
    flex-direction: column;
    justify-content: center;

    border-radius: 7px;
    
    background: #ffffff;
}

.extension__name_tables_container {
    display: flex;
    align-items: center;
}

.name_table__description {
    width: 420px;
    
    margin-top: 20px;

    font-size: 14px;
    font-style: italic;
    color: #9caeb6;
}
</style>