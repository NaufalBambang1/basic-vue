<template>
  <h2>{{ props }}</h2>
  <button @click="changeText">Ubah Text</button>
</template>

<script>
export default {
  name: "Header",
  props: ["props"],
  data() {
    return {
      newText: "ini data dari Header",
    };
  },
  methods: {
    changeText() {
      this.$emit("changeTitle", this.newText);
    },
  },
  emits: ["changeTitle"],
};
</script>
