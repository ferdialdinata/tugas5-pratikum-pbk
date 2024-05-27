<template>
    <q-footer class="bg-primary text-white text-center q-pa-md" elevated>
      <div>© 2024 My Online Store. All rights reserved.</div>
      <div>Follow us on:
        <q-icon name="fab fa-facebook" class="q-ml-sm" />
        <q-icon name="fab fa-twitter" class="q-ml-sm" />
        <q-icon name="fab fa-instagram" class="q-ml-sm" />
      </div>
    </q-footer>
  </template>
  
  <script>
  export default {
    name: 'Footer'
  }
  </script>
  
  <style scoped>
  .text-center {
    text-align: center;
  }
  .q-pa-md {
    padding: 16px;
  }
  .q-ml-sm {
    margin-left: 8px;
  }
  </style>
  