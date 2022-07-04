<template>
  <q-page class="flex flex-center">
    <img
      alt="Quasar logo"
      src="~assets/quasar-logo-vertical.svg"
      style="width: 200px; height: 200px">
    <div id="app">
      <jodit-editor v-model="content" />
    </div>
  </q-page>
</template>

<script setup>
import { ref } from 'vue'
import 'jodit/build/jodit.min.css'
import { JoditEditor } from 'jodit-vue'

const content = ref('')
content.value = '<h1>Hello Jodit Vue</h1>'

</script>
