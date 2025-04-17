<template>
    <main class="columns is-gapless is-multiline">
      <div class="column is-one-quarters">
        <BarraLateral />
      </div>
      <div class="column is-three-quarters">
        <FormularioComponent />
        <div class="lista">
          <TarefaComponent />
          <TarefaComponent />
          <TarefaComponent />
          <TarefaComponent />

        </div>
      </div>
    </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import BarraLateral from './components/BarraLateral.vue';
import FormularioComponent from './components/FormularioComponent.vue';
import TarefaComponent from './components/TarefaComponent.vue';

export default defineComponent({
  name: 'App',
  components: {
    BarraLateral,
    FormularioComponent,
    TarefaComponent
  }
});
</script>

<style>
.lista {
  padding: 1.5rem;
}
</style>
