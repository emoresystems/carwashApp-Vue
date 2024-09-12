<template>
  <div class="headersection">
    <h1>{{ heading }}</h1>
    <p>{{ description }}</p>
    <button @click="learnMore">Learn more</button>
  </div>

  <ServicesComponent />
  <ContactUs/>
</template>

<script>
import ServicesComponent from './components/ServicesComponent.vue'
import ContactUs from './components/ContactUs.vue'

export default {
  name: "App",

  components:{
    ServicesComponent,
    ContactUs
  },

  data() {
    return {
      heading: "Murema Carwash Services",
      description: "Best services in town",
      companyName: "Murema Carwash",
      aboutus:
        "At Murema Car Wash, we provide top-notch car cleaning and detailing services to keep your vehicle looking spotless and running at its best. Whether it's a quick exterior wash or a complete interior and exterior detailing, our dedicated team uses high-quality products and modern equipment to give your car the care it deserves.",
    };
  },
  methods: {
    learnMore() {
      alert(`welcome to ${this.companyName}, ${this.aboutus}`);
    },
  },
};
</script>

<style scoped>
.headersection {
  background-color: rgb(184, 184, 253);
  text-align: center;
  padding: 15px;
}
.headersection button {
  background-color: chartreuse;
  border: 0px;
  padding: 15px 40px;
  border-radius: 15px;
}
</style>
