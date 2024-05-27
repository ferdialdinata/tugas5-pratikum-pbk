<template>
    <q-header elevated>
      <q-toolbar>
        <q-btn flat round dense icon="menu" aria-label="Menu" @click="toggleDrawer" />
        <q-toolbar-title>
          <img src="path/to/logo.png" alt="Logo" height="40">
        </q-toolbar-title>
        <q-space />
        <q-btn flat round dense icon="shopping_cart" aria-label="Cart" @click="goToCart" />
      </q-toolbar>
    </q-header>
  </template>
  
  <script>
  export default {
    methods: {
      toggleDrawer() {
        this.$refs.drawer.toggle();
      },
      goToCart() {
        this.$router.push('/cart');
      }
    }
  }
  </script>
  
  <style scoped>
  q-toolbar-title {
    display: flex;
    align-items: center;
  }
  img {
    max-height: 40px;
  }
  </style>
  