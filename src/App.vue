<template>
  <div class="flex">
    <Sidebar />
    <Main />
  </div>
</template>

<script>
import Main from './components/Main.vue'
import Sidebar from './components/Sidebar.vue'
export default {
  components: {Sidebar, Main},
}
</script>

<style>

</style>