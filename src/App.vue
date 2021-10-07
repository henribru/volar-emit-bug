<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld :msg="'Hello Vue 3 + TypeScript + Vite'" @foo-bar="(foo) => console.log(foo)" @foo-baz="(foo) => console.log(foo)" />
</template>

<script lang="ts">
import { defineComponent } from '@vue/runtime-core'
import HelloWorld from './components/HelloWorld.vue'

export default defineComponent(
  {
    components: {
      HelloWorld
    },
    setup() {
      return { console }
    }
  }
)
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
