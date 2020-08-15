<template>
  <div id="app">
    <button class="button" v-on:click="openModal()">Click Here</button>
    <MyModal ref="myModal"></MyModal>
  </div>
</template>

<script>
import MyModal from "@/components/MyModal";

export default {
  name: 'App',
  components: {
    MyModal
  },
  methods:{
    openModal(){
      this.$refs.myModal.onOpen();
    }
  }
}
</script>

<style>
@import "./assets/style.css";
</style>
