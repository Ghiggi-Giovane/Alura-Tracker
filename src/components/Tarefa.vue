<template>
  <Box>
    <div class="columns">
      <div class="column is-7">
        {{ tarefa.descricao || "Tarefa sem Descrição" }}
      </div>
      <div class="column">
        <Cronometro :tempoEmSegundos="tarefa.duracaoEmSegundos" />
      </div>
    </div>
  </Box>
</template>

<script lang="ts">
import ITarefa from "@/interfaces/ITarefa";
import { defineComponent, PropType } from "vue";
import Cronometro from "./Cronometro.vue";
import Box from "./Box.vue";

export default defineComponent({
  name: "MeuTarefa",
  components: {
    Cronometro,
    Box,
  },

  props: {
    tarefa: {
      type: Object as PropType<ITarefa>,
      required: true,
    },
  },
});
</script>

<style scoped></style>
