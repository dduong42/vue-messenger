<template>
  <div class="row">
    <div class="col-3">
      <img v-bind:src="conversation.img_url" class="img-thumbnail">
    </div>
    <div class="col-9 text-truncate">
      <div class="row">
        <div class="col text-truncate">{{ conversation.title }}</div>
        <div class="col text-right">{{ conversation.when }}</div>
      </div>
      <div class="row">
        <div class="col text-truncate">
          {{ conversation.last_message }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'conversation',
  props: {
    conversation: Object
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
