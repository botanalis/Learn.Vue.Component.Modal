<template>
  <div class="modal" v-if="isActive">
    <div class="modal-content">
      <div class="modal-header">
        <span class="closeBtn" v-on:click.self="onClose()">&times;</span>
        <h2>Modal Header</h2>
      </div>
      <div class="modal-body">
        <p>Hello... I am a modal</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla repellendus nisi, sunt consectetur ipsa velit
          repudiandae aperiam modi quisquam nihil nam asperiores doloremque mollitia dolor deleniti quibusdam nemo
          commodi ab.
        </p>
      </div>
      <div class="modal-footer">
        <h3>Modal Footer</h3>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: "MyModal",
  data(){
    return {
      isActive: false
    }
  },
  methods:{
    onOpen(){
      this.isActive = true;
    },
    onClose(){
      console.log("close modal");
      this.isActive = false;
    }
  }
}
</script>

<style scoped>

</style>
