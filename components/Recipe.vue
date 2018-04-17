<template>
  <div class="col-md-3" style="margin: 10px">
    <nuxt-link :to="'Recepies/' + id">
      <div class="card" style="width: 18rem; padding: 10px;">
        <img
          class="card-img-top"
          :src="thumbnail"
          alt="Card image cap"
          width="100%"
          height="300px"
        >
        <div class="card-body">
          <p>{{previewText}}</p>
        </div>
      </div>
    </nuxt-link>
  </div>
</template>

<script>
  export default {
    props:['title', 'thumbnail', 'previewText', 'id']
  }
</script>
