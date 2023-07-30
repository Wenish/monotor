<template>
    <div class="text-4xl text-red-400 p-4">Hallo</div>
    <div>{{ data }}</div>
</template>
<script lang="ts" setup>
const trpc = useTrpc()

const data = await trpc.title.query()
</script>