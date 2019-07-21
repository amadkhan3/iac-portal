<template>
  <div id="app">
    <b-row>
      <b-col style="z-index:1000;">
        <Header />
      </b-col>
    </b-row>
    <b-row no-gutter>
      <b-col cols="2">
        <Sidebar />
      </b-col>
      <b-col cols="10">
        <Content />
      </b-col>
    </b-row>
  </div>
</template>

<script>

import Sidebar from './components/layout/Sidebar'
import Content from './components/layout/Content.vue'
import Header from './components/layout/Header.vue'

export default {
  name: 'app',
  components: {
    Sidebar,
    Content,
    Header
  },
  data () {
    return {
      menu: [
          {
              header: true,
              title: 'Main Navigation',
          },
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  overflow: hidden;
}
</style>
