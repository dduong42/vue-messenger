<template>
  <div class="col-2 d-block d-md-none border border-top-0">
    <template v-for="conversation in conversations">
      <conversation-small v-bind:conversation="conversation"/>
    </template>
  </div>
</template>

<script>
import ConversationSmall from './ConversationSmall.vue'

export default {
  name: 'conversation-list-small',
  components: {
    ConversationSmall
  },
  props: {
    conversations: Array
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
