<template>
  <div class="container">
    <div>
      <h1>Helloworld</h1>
      <h1 class="title">
        sms
      </h1>
        {{counter}} 
        <!-- {{counter123}} -->
        <button class="btn btn-sm btn-info" @click="storetest"> Store Test</button>
     
     </div>
    </div>
  
</template>

<script>
import {mapState, mapActions, mapGetters} from 'vuex'

export default {
  computed : {
  ...mapGetters('modules/crudAdmin',['counter','counter123']),
  ...mapState('modules/crudAdmin',['counter','counter123'])
  },

  methods : {
    ...mapActions('modules/crudAdmin',['readData']),
    storetest() {
      // this.readData({ test:'Hello'})
      this.counter
    },
  }
 
}
</script>

<style>

</style>

