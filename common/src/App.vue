<template>
  <div>
    <app-header :title="appTitle"></app-header>
    <app-content :items="items" @renew="renewItems"></app-content>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'

export default {
  components: { 
    AppHeader,
    AppContent
  },

  data() {
    return {
      appTitle: "Common Approach",
      items : [1,2,3,4]
    }
  },
  methods: {
    renewItems() {
      console.log("renewItems!!")
      this.items = [10,20,30,40]
    }
  }
}
</script>

<style>

</style>