<template>
  <div>
    <h1>My Items Page</h1>
    <div>
      <MyItem
      v-for="item in myRentals"
      :key="item.id"
      :item='item'/>
    </div>
  </div>
</template>

<script>
import {mapState} from "vuex";

export default {
  layout: 'no-nav',

  computed:{
     ...mapState(['myRentals'])
  }
}
</script>

<style scoped>
.container {
}
</style>
