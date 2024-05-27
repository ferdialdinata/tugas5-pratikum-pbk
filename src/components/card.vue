<template>
    <q-page padding>
      <q-gutter-md>
        <q-row>
          <q-col
            v-for="product in products"
            :key="product.id"
            cols="12"
            sm="6"
            md="4"
            lg="4"
          >
            <q-card flat bordered class="q-ma-md">
              <q-card-section>
                <q-img :src="product.image" class="product-image" />
                <div class="text-h6">{{ product.name }}</div>
                <div class="text-subtitle2 q-mt-xs">{{ product.description }}</div>
              </q-card-section>
            </q-card>
          </q-col>
        </q-row>
      </q-gutter-md>
    </q-page>
  </template>
  
  <script>
  export default {
    data() {
      return {
        products: [
          {
            id: 1,
            name: 'Produk A',
            description: 'Deskripsi singkat produk A.',
            image: 'https://th.bing.com/th/id/OIP.3xwhBDBIj9_w3rS6vzj0mAHaD4?w=1024&h=536&rs=1&pid=ImgDetMain'
          },
          {
            id: 2,
            name: 'Produk B',
            description: 'Deskripsi singkat produk B.',
            image: 'https://lh6.googleusercontent.com/-6zz1ok7b_Ak/UGsKPMAqpgI/AAAAAAADF9I/Q7Gstzd_uko/s1000/nike-lebron-10-id-preview-sprite-1-01.jpg'
          },
          {
            id: 3,
            name: 'Produk C',
            description: 'Deskripsi singkat produk C.',
            image: 'https://sneakerbardetroit.com/wp-content/uploads/2019/09/Nike-Air-Max-270-React-Just-Do-It-CT2203-001-Release-Date-768x493.jpg'
          }
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  .product-image {
    width: 100%;
    height: 200px;
    object-fit: cover;
  }
  .q-ma-md {
    margin: 16px;
  }
  </style>
  