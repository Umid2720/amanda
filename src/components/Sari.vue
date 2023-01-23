<template>
    <button class="sari">
        <p class="sari__title">{{ sariTitle }}</p>
        <h4 class="sari__result">{{ sariResult }}</h4>
    </button>
</template>

<script>
export default {
    props: {
        sariTitle: String,
        sariResult: String,
    }
}
</script>

<style>
.sari {
    width: 158px;
    height: 90px;
    display: flex;
    padding: 16px 20px;
    flex-direction: column;
    border: 1px solid #EAEAEA;
}
.sari__title {
    font-size: 16px;
    line-height: 21px;
    margin-bottom: 8px;
    color: var(--A2Color);
}
.sari__result{
    font-size: 22px;
    line-height: 29px;
}
</style>