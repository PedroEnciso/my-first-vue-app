<template>
  <div>
    <label for="message">Write a message:</label>
    <input ref="input" type="text" id="message" autocomplete="off" />
    <button @click="postMessage">Post!</button>
  </div>
  <MessageBoard :message="message" />
</template>
<script>
import MessageBoard from "./MessageBoard.vue";

let message = "";

export default {
  components: {
    MessageBoard,
  },
  methods: {
    postMessage() {
      this.message = this.$refs["input"].value;
      this.$refs["input"].value = "";
      console.log(message);
    },
  },
  data() {
    return {
      message,
    };
  },
};
</script>
<style></style>
