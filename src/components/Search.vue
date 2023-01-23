<template>
  <div class="search">
    <label class="flex">
        <img src="../assets/search.png" alt="search.png" width="19">
        <input type="text" class="search__input" placeholder="Search">
    </label>
  </div>
</template>

<script>
</script>

<style>

.search label{
    padding: 16px 22px;
    border-radius: 8px;
    border: 1px solid var(--EColor);
}

.search__input{
    flex: 1;
    margin-left: 10px;
}

.search__input::placeholder{
    font-size: 16px;
    line-height: 21px;
    color: var(--A2Color);
    font-family: 'DM Sans', sans-serif;
}
</style>