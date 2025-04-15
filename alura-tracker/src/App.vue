<template>
    <main class="columns is-gapless is-multiline">
      <div class="column is-one-quarters">
        <BarraLateral />
      </div>
      <div class="column is-three-quarters">
        <FormularioComponent />
      </div>
    </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import BarraLateral from './components/BarraLateral.vue';
import FormularioComponent from './components/FormularioComponent.vue';

export default defineComponent({
  name: 'App',
  components: {
    BarraLateral,
    FormularioComponent
  }
});
</script>

<style>

</style>
