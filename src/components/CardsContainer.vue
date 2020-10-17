<template>
  <main>
    <v-container class="body-container">
      <Filters></Filters>
    </v-container>
  </main>
</template>

<script>

import Filters from './Filters'

export default {
  name: 'CardsContainer',
  components: {
    Filters
  }
}
</script>

<style>
</style>