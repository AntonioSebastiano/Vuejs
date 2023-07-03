<template>
<div>
    <Navbar />
</div>
    
<div class="container">
    <h1>Home Page</h1>
    <div class="image-container">
        <h2>Python</h2>
    <img src="../assets/python.png" alt="Immagine PNG" />
    </div>
</div>



</template>

<script>
import Navbar from '@/components/Navbar.vue';

export default {
    name: 'HomePage',
    props: {
      msg: String
    },
    components:{
        Navbar,
    },
    methods: {

    },
  }
  </script>

<style>
body {
  background-image: url('../assets/walpaper.jpg');
  background-size: cover;
  background-position: center;
}


.image-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 300px; /* Altezza desiderata */
}

.image-container img {
  max-width: 100%;
  max-height: 100%;
}

</style>