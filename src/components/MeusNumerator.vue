<template>
  <section>
    <h3>Counter: {{ numerus }}</h3>
    <h3>Square: {{ quadrataNumerus }}</h3>

    <div>
      <button @click="numerus++">+1</button>
      <button @click="numerus--">-1</button>
    </div>
  </section>
</template>

<script lang="ts" setup>
import { computed, ref } from 'vue';

interface Props {
  valorem?: number;
}

const props = defineProps<Props>();

const numerus = ref(props.valorem ?? 10);

const quadrataNumerus = computed(() => numerus.value * numerus.value);
</script>
