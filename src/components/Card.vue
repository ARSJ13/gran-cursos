<template>
  <div class="card-container">
    <div class="card-description">
      <div class="card-image">
        <img :src="image" :alt="alt">
      </div>
      <div class="card-content">
        <h4>{{ title }}</h4>
        <p><span>by</span> {{ brand }}</p>
        <p>{{ description }}</p>
      </div>
    </div>
    <div class="card-price">
      <button
        class="price-rating"
        @click="countRating"
      >{{ rating }}<v-icon
        class="price-icon"
        color='#ffab00'
        small
      >mdi-star</v-icon></button>
      <p>{{ price }}</p>
      <span><v-icon small>mdi-cart-outline</v-icon> free shipping</span>
      <button
        class="price-heart"
      ><v-icon
        class="icon"
        color="#fff"
        small
        >mdi-heart-outline</v-icon>
      wishlist</button>
      <button
        class="price-shopping"
      ><v-icon
        class="icon"
        color="#fff"
        small
        >mdi-shopping-outline</v-icon>
      add to cart</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ['title', 'brand', 'description', 'rating', 'price', 'image', 'alt'],
  methods: {
    countRating(){
      let count = this.rating++
      return count
    }
  }
}
</script>

<style>
.card-container{
  display: flex;
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;
  background: #F4F5F7;
  color: #253858;
  max-height: 200px;
}
.card-description{
  display: flex;
}
.card-image>img{
  height: 150px;
  width: 150px;
  margin: 0.5rem 0.5rem;
}
.card-content{
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 0.5rem;
}
.card-content>h4{
  text-transform: capitalize;
  font-weight: 400;
}
.card-content>p{
  font-size: 0.8rem;
  line-height: 1.2rem;
}
.card-content>p:nth-child(2n){
  margin: 0.5rem 0;
  text-transform: uppercase;
}
.card-content>p>span{
  opacity: 0.6;
  text-transform: capitalize;
}
.card-price{
  min-width: 200px;
  border-left: 1px solid #DADADA;
  padding: 1rem;

  display: grid;
  row-gap: 5px;
}
.price-rating{
  width: 2.8rem;
  height: 1.5rem;
  border-radius: 5px;
  background: #0052CC;
  color: #fff;
  font-size: 0.8rem;
  font-weight: 600;
  justify-self: end;
}
.price-icon{
  margin-left: 3px;
}
.card-price>p{
  justify-self: center;
}
.card-price>span{
  opacity: 0.6;
  font-size: 0.8rem;
  justify-self: center;
}
.price-heart{
  background: #6554C0;
  color: #fff;
  font-weight: 700;
  text-transform: uppercase;
  font-size: 0.8rem;
  border-radius: 5px;
}
.price-shopping{
  background: #36B37E;
  color: #fff;
  font-weight: 700;
  text-transform: uppercase;
  font-size: 0.8rem;
  border-radius: 5px;
}
.icon{
  margin-right: 3px;
}
</style>