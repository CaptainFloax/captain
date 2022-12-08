<script setup lang="ts">import { ref } from 'vue';

defineProps<{
  msg: string
}>()

const name = ref<string>("Coucou");

</script>

<template>
  <div class="greetings">
    <h1>{{ name }}</h1>
    <input type="text" v-model="name"/>
    <h3>
      Hey !
    </h3>
  </div>
</template>

<style scoped lang="scss">
  @use './_HelloWordl.scss';
</style>
