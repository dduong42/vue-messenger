<template>
  <div id="app">
    <div class="container">
      <div class="row text-center">
        <div class="col-5 d-none d-md-block border">
          <div class="row">
            <div class="col">
              <i class="fas fa-cog fa-2x"></i>
            </div>
            <div class="col">
              Messenger
            </div>
            <div class="col">
              <i class="fas fa-edit fa-2x"></i>
            </div>
          </div>
        </div>
        <div class="col-2 d-block d-md-none border">
          <i class="fas fa-edit fa-2x"></i>
        </div>
        <div class="col right-panel border border-left-0">
          Lorem ipsum
        </div>
      </div>
      <main-row v-bind:conversations="conversations"/>
    </div>
  </div>
</template>

<script>
import MainRow from './components/MainRow.vue'

export default {
  name: 'app',
  components: {
    MainRow
  },
  data () {
    return {
      conversations: [
        {
          img_url: "https://placekitten.com/50/50",
          title: "Miaou 1 miaou miaou miaou miaou miaou miaou",
          when: "12:51pm",
          last_message: "Miaou miaou miaou miaou miaou miaou miaou"
        },
        {
          img_url: "https://placekitten.com/50/50",
          title: "Miaou 2 miaou miaou miaou miaou miaou miaou",
          when: "12:51pm",
          last_message: "Miaou miaou miaou miaou miaou miaou miaou"
        },
        {
          img_url: "https://placekitten.com/50/50",
          title: "Miaou 3 miaou miaou miaou miaou miaou miaou",
          when: "12:51pm",
          last_message: "Miaou miaou miaou miaou miaou miaou miaou"
        }
      ]
    }
  },
}
</script>

<style>
</style>
