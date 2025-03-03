<script setup>
import { onBeforeMount } from 'vue'
import ItemContainer from '@/components/ItemContainer.vue'
import useGlobalStore from '@/stores/index.js'

const globalStore = useGlobalStore()

onBeforeMount(() => {
  globalStore.rememberTime()
})
</script>

<template>
  <ItemContainer father-component="item"></ItemContainer>
</template>

<style scoped lang="less"></style>
