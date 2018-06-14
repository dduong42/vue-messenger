<template>
  <div class="row">
    <conversation-list v-bind:conversations="conversations"/>
    <conversation-list-small v-bind:conversations="conversations"/>
    <div class="col right-panel border border-left-0 border-top-0">
      Lorem ipsum
    </div>
  </div>
</template>

<script>
import ConversationList from './ConversationList.vue'
import ConversationListSmall from './ConversationListSmall.vue'


export default {
  name: 'main-row',
  components: {
    ConversationList,
    ConversationListSmall
  },
  props: {
    conversations: Array
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
