<template>
    <div class="box">
        <div class="columns">
            <div class="column is-8" role="form" aria-label="Formulário para a ciração de uma nova tarefa">
                <input type="text" class="input" placeholder="Qual tarefa você deseja iniciar?" />
            </div>
            <div class="column">
                <TemporizadorComponent @aoTemporizadorfinalizado="finalizarTarefa"/>
            </div>
        </div>
    </div>

</template>

<script lang="ts">

import { defineComponent } from 'vue';
import TemporizadorComponent from './TemporizadorComponent.vue';

export default defineComponent({
    name: 'FormularioComponent',
    components: {
        TemporizadorComponent
    },
    methods: {
        finalizarTarefa (tempoDecorrido: number) : void {
            console.log('tempo da tarefa:', tempoDecorrido)
            
        }
    }
});
</script>