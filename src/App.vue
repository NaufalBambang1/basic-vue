<template>
  <!-- Data & Methods -->
  <!-- <h2>Nama: {{ nama }}</h2>
  <button v-on:click="changeName">Change name</button> -->
  <!-- bisa juga menggunakan @click pada changeName -->

  <!-- Data Binding -->
  <!-- <a v-bind:href="url">Go To Google</a> -->
  <!-- bisa juga disingkat menjadi :href data binding -->

  <!-- Two-way Data Binding -->
  <!-- <input type="text" v-model="nama" />
  {{ nama }} -->

  <!-- For Loops and Condiont -->
  <!-- <div v-if="products.length">
    <ul>
      <li v-for="items in products" :key="id">{{ items.title }} - {{ items.price }}</li>
    </ul>
  </div>
  <div v-else>
    <p>Ga ada datanya bro</p>
  </div> -->

  <!-- Computed -->
  <input type="text" v-model="cari" placeholder="cari" />
  <ul>
    <li v-for="items in cariData" :key="id">{{ items.title }} - {{ items.price }}</li>
  </ul>

  <!-- Componenet & props -->
  <!-- <Header @changeTitle="ubahText" :props="text" /> -->
</template>

<script>
// import Header from "@/components/Header.vue";
export default {
  name: "App",
  // Data & Methods ---------------------
  // data() {
  //   return {
  //     nama: "Naufal Bambang",
  //   };
  // },
  // methods: {
  //   changeName() {
  //     this.nama = "Manuka";
  //   },
  // },
  // Data Binding ------------------------------
  // data() {
  //   return {
  //     url: "https://www.google.com/",
  //   };
  // },
  // Two-way Data Binding ---------------------------
  // data() {
  //   return {
  //     nama: "",
  //   };
  // },
  // For Loops and condition --------------------------
  // data() {
  //   return {
  //     products: [
  //       { id: 1, title: "Product-1", price: 1000 },
  //       { id: 2, title: "Product-2", price: 2000 },
  //       { id: 3, title: "Product-3", price: 3000 },
  //       { id: 4, title: "Product-4", price: 4000 },
  //       { id: 5, title: "Product-5", price: 5000 },
  //     ],
  //   };
  // },

  // data() {
  //   return {
  //     cari: "",
  //     products: [],
  //   };
  // },
  // Lifecycle hook
  // created() {
  //   this.products = [
  //     { id: 1, title: "Product-1", price: 1000 },
  //     { id: 2, title: "Product-2", price: 2000 },
  //     { id: 3, title: "Product-3", price: 3000 },
  //     { id: 4, title: "Product-4", price: 4000 },
  //     { id: 5, title: "Product-5", price: 5000 },
  //   ];
  // },
  // computed: {
  //   cariData() {
  //     return this.products.filter((item) => {
  //       return item.title.match(this.cari);
  //     });
  //   },
  // },

  // components: {
  //   Header,
  // },
  // data() {
  //   return {
  //     text: "Halo aku data dari app",
  //   };
  // },
  // methods: {
  //   ubahText(newText) {
  //     this.text = newText;
  //   },
  // },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

a {
  text-decoration: none;
  color: red;
  font-weight: 700;
}
</style>
