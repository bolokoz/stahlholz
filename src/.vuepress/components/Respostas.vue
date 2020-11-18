<template>
  <v-expansion-panels>
    <v-expansion-panel v-for="resposta in respostas" :key="resposta.id">
      <v-expansion-panel-header expand-icon="mdi-menu-down">
        {{ resposta.alternativa }}
        <template v-slot:actions v-if="resposta.correta">
            <v-icon color="teal">
              mdi-check
            </v-icon>
          </template>
      </v-expansion-panel-header>
      <v-expansion-panel-content>
        {{ resposta.solucao }}
      </v-expansion-panel-content>
    </v-expansion-panel>
  </v-expansion-panels>
</template>

<script>
export default {
  props: ["respostas"],
};
</script>

<style>
</style>template