<template>
    <q-page>
      <div class="q-pa-md">
        <q-card flat bordered class="my-card">
          <q-img src="path/to/hero-image.jpg" style="height: 400px;">
            <div class="absolute-bottom text-h5 text-white text-center">
              <q-btn color="primary" label="Belanja Sekarang" @click="goToShop" />
            </div>
          </q-img>
        </q-card>
      </div>
    </q-page>
  </template>
  
  <script>
  export default {
    methods: {
      goToShop() {
        this.$router.push('/shop');
      }
    }
  }
  </script>
  
  <style scoped>
  .my-card {
    position: relative;
    overflow: hidden;
  }
  </style>
  