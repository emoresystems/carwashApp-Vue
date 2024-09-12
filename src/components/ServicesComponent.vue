<template>
  <h1>Services Section</h1>
  <div class="services">
    <h2>{{ servicename }}</h2>
    <p>{{ description }}</p>
    <h3>{{ price }}</h3>
  </div>
</template>

<script>
export default {
  name: "ServicesComponent",

  data() {
    return {
      servicename: "Body wash",
      description: "Medium sized cars whole body wash",
      price: "200",
    };
  },
};
</script>

<style scoped>
h1 {
  text-align: center;
  color: rgb(136, 136, 254);
}

.services {
  background-color: chartreuse;
  text-align: center;
  padding: 10px;
  width: 250px;
  height: 250px;
}
</style>
