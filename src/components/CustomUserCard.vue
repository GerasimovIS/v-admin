<template>
  <div class="col-md-12">
    <div class="card">
      <div class="card-header" style="background-color: lightblue;">
        <h5><strong>{{user.name}}</strong></h5>
      </div>
      <div class="card-body">
        <p class="card-text">
          <ul class="list-group list-group-flush">
            <li class="list-group-item"><strong>Username</strong> : {{user.username}}</li>
            <li class="list-group-item"><strong>Email</strong> : {{user.email}}</li>
            <li class="list-group-item"><strong>Phone</strong> : {{user.phone}}</li>
            <li class="list-group-item"><strong>Website</strong> : {{user.website}}</li>
          </ul>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['user']
}
</script>

