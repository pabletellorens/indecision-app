<template>
  <div class="p-4 flex-1 overflow-y-auto">
    <div class="flex flex-col space-y-2">
      <ChatBullula :meus-est="true" nuntius="¿Salimos?" />

      <ChatBullula :meus-est="false" 
      nuntius="no" 
      imago="https://yesno.wtf/assets/no/24-159febcfd655625c38c147b65e5be565.gif"/>
    </div>
  </div>
</template>

<script lang="ts" setup>
import ChatBullula from './ChatBullula.vue';
</script>
