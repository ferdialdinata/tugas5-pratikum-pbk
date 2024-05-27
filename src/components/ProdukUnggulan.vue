<template>
    <q-page>
      <q-card flat bordered class="q-ma-md">
        <q-card-section>
          <div class="text-h6">Produk Unggulan</div>
        </q-card-section>
        <q-card-section>
          <q-carousel animated height="300px">
            <q-carousel-slide
              v-for="product in products"
              :key="product.id"
              :name="product.name"
              :img-src="product.image"
            >
              <div class="text-h5 text-white">{{ product.name }}</div>
            </q-carousel-slide>
          </q-carousel>
        </q-card-section>
      </q-card>
    </q-page>
  </template>
  
  <script>
  export default {
    data() {
      return {
        products: [
          { id: 1, name: 'Produk A', image: 'path/to/product-a.jpg' },
          { id: 2, name: 'Produk B', image: 'path/to/product-b.jpg' },
          // Tambahkan produk lain sesuai kebutuhan
        ]
      }
    }
  }
  </script>
  