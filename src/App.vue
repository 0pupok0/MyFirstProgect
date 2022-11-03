<template>
  <div>
    <header-comp></header-comp>
    <div class="content">
      <table-comp @Sp1="ScrollTo('p1')"></table-comp>
      <text-comp></text-comp>
      <button-comp></button-comp>
      
    </div>
  </div>
</template>

<script>
import headerComp from "@/components/headerComp.vue"
import textComp from "@/components/textComp.vue"
import tableComp from "@/components/tableComp.vue"
import buttonComp from "@/components/buttonComp.vue"
export default {
  name: 'App',
  components: {
    headerComp, textComp, tableComp, buttonComp
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #f7d0d0;
  height: fit-content;
  min-height: 100vh;
}

.content {
  display: flex;
  flex-direction: row;
}
</style>
