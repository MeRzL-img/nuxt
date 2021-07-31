<template lang="html">
    <button class="button">
        <slot />
    </button>
</template>
<script>
export default {

}
</script>
<style scoped lang="scss">
.button {
    width: 150px;
    height: 55px;

    border-radius: 5%;
    border: none;

    font-size: 14px;

    color: #eef0f2;

    background: #061e37;

    transition: 0.4s;
}

.button:hover {
    box-shadow: 0.4em 0.4em 5px rgba(122,122,122,0.5);
    cursor: pointer
}
</style>