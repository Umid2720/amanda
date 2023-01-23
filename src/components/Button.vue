<template>
  <button class="button">
    <slot></slot>
  </button>
</template>

<script>
export default {

}
</script>

<style>
.button{
    font-size: 16px;
    padding: 16px 24px;
    color: var(--A2Color);
    border: 1px solid var(--EColor);
}
.button:hover{
    color: var(--white);
    background-color: var(--purple);
}
</style>