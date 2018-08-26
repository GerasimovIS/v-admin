<template>
  <div class="row">
    <div class="com-sm-12">
      <CustomImgCard 
        v-for="(item, index) in data"
        :key="index"
        :item="item">
      </CustomImgCard>
    </div>
  </div>
</template>

<script>
import CustomImgCard from '../components/CustomImgCard.vue';

export default {
  components: {
    CustomImgCard
  },
  data() {
    return {
      data: null
    }
  },
  methods: {
    loadData() {
      fetch('https://jsonplaceholder.typicode.com/albums/1/photos')
        .then(res => res.json())
        .then(data => this.data = data)
    }
  },
  mounted() {
    this.loadData()
  }
}
</script>
