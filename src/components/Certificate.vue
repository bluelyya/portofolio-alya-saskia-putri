<script setup>
import sertifikat1 from '../assets/sertifikat1.jpeg'
import sertifikat2 from '../assets/sertifikat2.jpeg'
import sertifikat3 from '../assets/sertifikat3.jpeg'

const certificates = [
  {
    title:'Python',
    image: sertifikat1
  },
  {
    title:'SDGs',
    image: sertifikat2
  },
  {
    title:'SDGs',
    image: sertifikat3
  }
]
</script>

<template>

<section id="certificate" class="section">

  <h2 class="section-title">
    Sertifikat
  </h2>

  <div class="certificate-grid">

    <div
      v-for="item in certificates"
      :key="item.title"
      class="certificate-card"
    >

      <img
        :src="item.image"
        :alt="item.title"
      >

      <h3>
        {{ item.title }}
      </h3>

    </div>

  </div>

</section>

</template>