<script setup>
    const props = defineProps(['tarefasPendentes'])
</script>
<template>
    <header class="p-5 mb-4 mt-4 bg-light rounded-3">
        <h1>Minhas Tarefas</h1>
        <p v-if="props.tarefasPendentes > 1">
            Você possui {{ props.tarefasPendentes }} tarefas pendentes
        </p>
        <p v-else-if="props.tarefasPendentes === 1">Você possui 1 tarefa pendente</p>
        <p v-else>Você não possui tarefas pendentes</p>
    </header>
</template>