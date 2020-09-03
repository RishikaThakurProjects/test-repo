<template>
  <div class="container">
    <div>
<<<<<<< HEAD
      <h1>hello</h1>
=======
      <h1>Helloworld</h1>
>>>>>>> 79802efbf5fd43a25ff35edb9b7d7b83c565a929
      <h1 class="title">
        sms
      </h1>
      <h1>
        clone</h1>
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

