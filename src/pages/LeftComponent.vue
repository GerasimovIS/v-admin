<template>
  <div class="row">
    <CustomUserCard 
      v-for="(user, index) in users"
      :key="index"
      :user="user">
    </CustomUserCard>
  </div>
</template>

<script>
import CustomUserCard from '../components/CustomUserCard.vue';

export default {
  components: {
    CustomUserCard
  },
  data() {
    return {
      users: null
    }
  },
  methods: {
    loadUsers() {
      fetch('https://jsonplaceholder.typicode.com/users')
        .then(res => res.json())
        .then(data => this.users = data)
    }
  },
  mounted() {
    this.loadUsers()
  }
}
</script>
