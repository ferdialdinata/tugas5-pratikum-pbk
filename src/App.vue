<template>
  <q-layout view="hHh lpR fFf">
    <Header />
    <q-page-container>
    
      <carousel/>
      <card/>
    </q-page-container>
   <foter/>
  </q-layout>
</template>

<script>
import Header from './components/Header.vue'
import carousel from './components/Carouse.vue'
import card from './components/card.vue'
import foter from './components/Footer.vue'


export default {
  components: {
    Header,
    carousel,
    card,
    foter,

  }
}
</script>
