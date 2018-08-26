<template>
  <div class="card">
    <img class="card-img-top" :src="item.url" alt="">
    <div class="card-body">
      <div class="card-title">
        <h5>{{item.title}}</h5>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['item']
}
</script>

