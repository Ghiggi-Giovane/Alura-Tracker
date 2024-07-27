<template>
  <div class="projetos">
    <h1 class="title">Projetos</h1>
    <router-view></router-view>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "MeuProjetos",
});
</script>

<style scoped>
.projetos {
  padding: 1.25rem;
  background-color: var(--bg-primario);
  color: var(--texto-primario);
}
.title {
  background-color: var(--bg-primario);
  color: var(--texto-primario);
}
</style>
