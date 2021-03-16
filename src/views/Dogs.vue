<template>
    <div>
        <h1>Dogs for Adoption
        <b-table striped hover :items="dogs"/>
        </h1>
    </div>
</template>
<script>

import dogs from '@/data/Dogs'

export default {
  data () {
    return {
      dogs
    }
  }
}
</script>
