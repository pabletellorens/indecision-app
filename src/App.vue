<template>
  <h1>Mi primera app de Vue</h1>

  <h1 class="text-3xl font-bold underline">Hello world!</h1>

  <MeusNumerator :valorem="5" />

  <MeusNumeratorScript :valorem="8" />

  <MeusNumeratorScript2 :valorem="9" />
</template>

<script lang="ts" setup>
import MeusNumeratorScript2 from './components/meus-numerator-script/MeusNumeratorScript2.vue';
import MeusNumerator from './components/MeusNumerator.vue';
import MeusNumeratorScript from './components/MeusNumeratorScript.vue';
</script>
