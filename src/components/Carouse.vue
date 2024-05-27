<template>
    <q-carousel
      animated
      v-model="slide"
      infinite
      navigation
      arrows
      :autoplay="5000"
    >
      <q-carousel-slide
        v-for="(image, index) in images"
        :name="index"
        :img-src="image.src"
        key="index"
      >
        <!-- Caption untuk setiap gambar -->
        <div class="caption">{{ image.caption }}</div>
      </q-carousel-slide>
    </q-carousel>
  </template>
  
  <script>
  export default {
    name: 'MyCarousel',
    data() {
      return {
        slide: 0,
        images: [
          {
            src: 'https://c.static-nike.com/a/images/f_auto/w_1920,c_limit/nni8ipthzexjynxjdm8j/1021-homepage-apla-xa.jpg',
            caption: 'NEW PRODUCK'
          },
          {
            src: 'https://sneakerbardetroit.com/wp-content/uploads/2020/03/Nike-Air-Max-270-React-White-Black-CT1264-101-Release-Date-4.jpg',
            caption: 'NEW PRODUCK'
          },
          {
            src: 'https://th.bing.com/th/id/OIP.cowQq4EQceqDBsIg8Th1RAHaFM?w=1140&h=800&rs=1&pid=ImgDetMain',
            caption: 'NEW PRODUCK'
          },
          {
            src: 'https://sneakernews.com/wp-content/uploads/2019/10/nike-air-max-270-react-camo-CT5528-001-4.jpg',
            caption: 'NEW PRODUCK'
          },
          {
            src: 'https://sneakernews.com/wp-content/uploads/2019/10/nike-air-max-270-react-camo-CT5528-001-6.jpg',
            caption: 'NEW PRODUCK'
          },
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  .q-carousel {
    height: 500px;
    width: 1500px;
  }
  
  .q-carousel-slide {
    background-position: center;
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  
  .caption {
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    background-color: rgba(0, 0, 0, 0.5);
    color: #fff;
    padding: 10px;
    border-radius: 10px;
    font-size: 30px;
  }
  </style>