<template>
  <div class="card w-100">
    <router-link class="mt-4 ml-4" :to="{ name: 'bookable', params: { id } }">
      <h5 class="card-title">{{ title }}</h5>
    </router-link>
    <div class="card-body">
      <p class="card-text">{{ description }}</p>
    </div>
  </div>
</template>


<script>
export default {
  props: { title: String, description: String, id: Number },
};
</script>