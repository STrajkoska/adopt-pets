<template>
    <div>
      <h1>Cats for Adoption</h1>
      <b-table striped hover :items="cats">
         <template v-slot:name="data" >
           <router-link :to="'/pets/${data.index}'">
               {{ data.value }}
           </router-link>
         </template>
      </b-table>
    </div>
</template>

<script>
import cats from '@/data/Cats'

export default {
  data () {
    return {
      cats
    }
  }
}
</script>
