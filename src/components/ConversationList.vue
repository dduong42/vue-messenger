<template>
  <div class="col-5 d-none d-md-block border border-top-0">
    <div class="row">
      <input type="text" class="form-control form-control-sm" placeholder="Search Messenger">
    </div>
    <template v-for="conversation in conversations" >
      <conversation v-bind:conversation="conversation"/>
    </template>
  </div>
</template>

<script>
import Conversation from './Conversation.vue'

export default {
  name: 'conversation-list',
  components: {
    Conversation
  },
  props: {
    conversations: Array
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
