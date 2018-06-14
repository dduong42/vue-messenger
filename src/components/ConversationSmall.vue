<template>
  <div class="row">
    <div class="col">
      <img v-bind:src="conversation.img_url" class="img-thumbnail">
    </div>
  </div>
</template>

<script>
export default {
  name: 'conversation-small',
  props: {
    conversation: Object
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
