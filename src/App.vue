<script setup>

const images = [
 {
    image: 'https://picsum.photos/400/200?random=1',
    alt: 'Random Image 1',
    title: 'Card Title 1',
    description: 'This is a description for card 1.',
    link: 'https://example.com/card1'
  },
  {
    image: 'https://picsum.photos/400/200?random=2',
    alt: 'Random Image 2',
    title: 'Card Title 2',
    description: 'This is a description for card 2.',
    link: 'https://example.com/card2'
  },
  {
    image: 'https://picsum.photos/400/200?random=3',
    alt: 'Random Image 3',
    title: 'Card Title 3',
    description: 'This is a description for card 3.',
    link: 'https://example.com/card3'
  },
 
];

</script>

<template>



<section class="container py-5">
  <div class="row g-4">
    <!-- Card 1 -->
    <div class="col-md-4">
      <div class="card h-100">
        <img :src="images[0].image" class="card-img-top" :alt="images[0].alt">
        <div class="card-body">
          <h5 class="card-title">{{ images[0].title }}</h5>
          <p class="card-text">{{ images[0].description }}.</p>
          <a :href="images[0].link" class="btn btn-primary">Learn More</a>
        </div>
      </div>
    </div>

    <!-- Card 2 -->
    <div class="col-md-4">
      <div class="card h-100">
        <img :src="images[1].image" class="card-img-top" :alt="images[1].alt">
        <div class="card-body">
          <h5 class="card-title">{{ images[1].title }}</h5>
          <p class="card-text">{{ images[1].description }}</p>
          <a :href="images[1].link" class="btn btn-primary">Learn More</a>
        </div>
      </div>
    </div>

    <!-- Card 3 -->
    <div class="col-md-4">
      <div class="card h-100">
        <img :src="images[2].image" class="card-img-top" alt="{{ images[2].alt }}">
        <div class="card-body">
          <h5 class="card-title">{{ images[2].title }}</h5>
          <p class="card-text">{{ images[2].description }}</p>
          <a :href="images[2].link" class="btn btn-primary">Learn More</a>
        </div>
      </div>
    </div>
  </div>
</section>



</template>

 
<style scoped>

</style>
