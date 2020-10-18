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
footer{
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;
}
</style>