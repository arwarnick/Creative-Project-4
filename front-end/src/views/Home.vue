<template>
<div class="home">
  <section class="image-gallery">
    <div class="image" v-for="item in items" :key="item.id">
      <img :src="item.path" />
      <h2>{{item.title}}</h2>
    </div>
  </section>
</div>
</template>

<style scoped>
.image h2 {
  font-family: "Arial Black", Gadget, sans-serif;
}

.home {
  display: flex;
  justify-content: center;
  margin-top: 70px;
}

.image-gallery {
  display: flex;
}

@media only screen and (min-width: 1024px) {
}

@media only screen and (max-width: 1023px) and (min-width: 768px) {
  .image-gallery {
    flex-direction: column;
  }
}

@media only screen and (max-width: 767px) and (min-width: 540px) {
  .image-gallery {
    flex-direction: column;
  }
}

</style>


<script>
import axios from 'axios';
export default {
  name: 'Home',
  data() {
    return {
    items: [],
    }
  },
  created() {
    this.getItems();
  },
  methods: {                                                                                                                  async getItems() {
      try {
        let response = await axios.get("/api/items");
        this.items = response.data;
        return true;
      } catch (error) {
        console.log(error);
      }
    },
  }
} 
</script>

