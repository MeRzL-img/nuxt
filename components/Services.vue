<template lang="html">
    <section class="services">
        <DTitle class="services__title" />
        <DTxt class="services__text" />
        <div class="services__tables">
            <DTable />
            <DTable />
            <DTable />
            <DTable />
            <DTable class="table__text--down" />
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
    }
}
</script>
<style scoped lang="scss">
.services {
    max-height: 1400px;
    
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
</style>