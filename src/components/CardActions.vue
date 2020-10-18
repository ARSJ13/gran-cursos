<template>
  <header class="card-actions-container">
    <div class="card-actions-title">
      <h3>card actions</h3>
      <div class="card-actions-map">
        <v-icon small>mdi-home-outline</v-icon>
        <v-icon>mdi-chevron-right</v-icon>
        <span>eCommerce</span>
        <v-icon>mdi-chevron-right</v-icon>
        <span>Eletronics</span>
      </div>
    </div>
    <div class="card-actions-config">
      <button><v-icon color="#fff">mdi-cog-outline</v-icon></button>
    </div>
  </header>
</template>

<script>
export default {
  name: 'CardActions'

}
</script>

<style>
header.card-actions-container{
  display: flex;
  justify-content: space-between;
  margin: 1rem 0;
}
.card-actions-title{
  display: flex;
  align-items: center;
}
.card-actions-title>h3{
  text-transform: capitalize;
  border-right: 1px solid #979797;
  font-weight: 400;
  padding-right: 1rem;
}
.card-actions-map{
  padding-left: 1rem;
  font-size: 0.8rem;
}
.card-actions-config{
  background: #091E42;
  padding: 5px;
  border-radius: 50%;
}
</style>