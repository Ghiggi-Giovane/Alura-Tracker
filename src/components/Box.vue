<template>
  <div class="box has-text-weight-bold">
    <!--  Slot quer dizer que o que estiver dentro da TAG BOX onde eu estou importando ele, vai renderizar aqui dentro-->
    <slot></slot>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "MeuBox",
});
</script>

<style scoped>
.box {
  background: darkgray;
  color: black;
}
</style>
