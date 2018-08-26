<template>
  <div class="row">
    <div class="col-md-6">
      <LeftComponent></LeftComponent>
    </div>
    <div class="col-md-6">
      <RightComponent></RightComponent>
    </div>
  </div>
</template>

<script>
import LeftComponent from './LeftComponent.vue';
import RightComponent from './RightComponent.vue';

export default {
  components: {
    LeftComponent,
    RightComponent
  }
}
</script>

