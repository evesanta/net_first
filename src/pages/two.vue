<template>
  <section class="container">
    <div>
      <logo/>
      <h1 class="title">変更しmした！</h1>
      <h2 class="subtitle">Nuxt TypeScript Project</h2>
      <input v-model="hatena">
      <p>{{hatena}}</p>
    </div>
  </section>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Logo from '../components/Logo.vue'

@Component({
  data() {
    return {
      value: 'hello',
      hatena: '',
    }
  },
  components: {
    Logo,
  },
})
export default class Index extends Vue {}
</script>

<style scoped>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  display: block;
  font-weight: 300;
  font-size: 50px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
