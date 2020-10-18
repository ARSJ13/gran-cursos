<template>
  <footer>
     <div class="text-center">
      <v-pagination
        class='page'
        v-model="page"
        :length="5"
        circle
      ></v-pagination>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  data(){
    return {
      page: 1
    }
  }
}
</script>

<style>

</style>