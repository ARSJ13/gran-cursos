<template>
  <div class="star-container">
    <div class="star">
      <v-icon
        v-for="c in check"
        :key="c"
        color='#ffab00'
      >mdi-star</v-icon>
      <v-icon
        v-for="n in out"
        :key="n"
        color="#A5ADBA"
      >mdi-star-outline</v-icon>
      <p>& up</p>
    </div>
    <div class="amount">
      {{ amount }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'Rating',
  props: ['check', 'out', 'amount']

}
</script>

<style>
.star-container{
  display: flex;
  justify-content: space-between;
  margin-bottom: 0.5rem;
}
.star{
  display: flex;
  align-items: center;
}
.star>p{
  margin-left: 1rem;
  text-transform: capitalize;
}
</style>