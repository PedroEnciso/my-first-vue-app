<template>
  <div class="message_board">
    <p class="message">{{ message }}</p>
  </div>
</template>
<script>
export default {
  props: ["message"],
};
</script>
<style>
.message_board {
  max-width: 400px;
  border-radius: 10px;
  margin: 40px auto 0px;
  padding: 15px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}

.message {
  font-size: 1.2rem;
  font-weight: 500;
  color: salmon;
}
</style>
