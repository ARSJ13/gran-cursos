<template>
  <section>
    <div class="filter-title">
      <h4>filters</h4>
    </div>
    <div class="filter-container">
      <div class="radio">
        <h4 class="radio-title">multi radio</h4>
        <form class="radio-form">
          <span><input type="radio" value="$10" v-model="check">{{values[0]}}</span>
          <span><input type="radio" value="$10-$100" v-model="check">{{values[1]}}</span>
          <span><input type="radio" value="$100-$500" v-model="check">{{values[2]}}</span>
          <span><input type="radio" value="$500" v-model="check">{{values[3]}}</span>
          <span><input type="radio" value="All" v-model="check">{{values[4]}}</span>
        </form>
        <hr/>
      </div>
      <div class="range">
        <div class="range-title-box">
          <h4 class="range-title">slider</h4>
          <span>1.99 - 4098</span>
        </div>
        <form class="range-form">
          <span><input type="range"></span>
        </form>
        <hr/>
      </div>
      <div class="check">
        <h4 class="check-title">category</h4>
        <form class="check-form" v-for="(item, id) in category" :key="id">
          <span><input type="checkbox">{{ item.name }}</span>
          <span>{{ item.amount }}</span>
        </form>
        <hr/>
      </div>
      <div class="check">
        <h4 class="check-title">brand</h4>
        <form class="check-form" v-for="(item, id) in brand" :key="id">
          <span><input type="checkbox">{{ item.name }}</span>
          <span>{{ item.amount }}</span>
        </form>
        <hr/>
      </div>
    </div>
  </section>  
</template>

<script>
export default {
  name: "Filters",
  data(){
    return{
      check: '$10',
      values: ['$10', '$10-$100', '$100-$500', '$500', 'All'],
      category: [
        {name: 'Cell Phones', amount: 1920},
        {name: 'Computers & Tablets', amount: 1820},
        {name: 'Cell Phone Accessories', amount: 462},
        {name: 'Appliances', amount: 6556},
        {name: 'Audio', amount: 120},
        {name: 'iPhone Accessories', amount: 353},
        {name: 'Cameras & Camcorders', amount: 45},
        {name: 'iPhone Cases & Clips', amount: 456},
        {name: 'TV & Home Theater', amount: 55},
        {name: 'Small Kitchen Appliances', amount: 10}
      ],
      brand: [
        {name: 'Insigni', amount: 220},
        {name: 'Samsung', amount: 120},
        {name: 'Apple', amount: 320},
        {name: 'HP', amount: 32},
        {name: 'Sony', amount: 520},
        {name: 'Metra', amount: 55},
        {name: 'Dyne', amount: 120},
        {name: 'LG', amount: 98},
        {name: 'Canon', amount: 99},
        {name: 'Speck', amount: 575}
      ]
    }
  }

}
</script>

<style>
hr{
  margin: 1rem 0;
}
.filter-title>h4{
  font-size: 1.5rem;
  margin-bottom: 1rem;
  text-transform: capitalize;
  font-weight: 300;

}
.filter-container{
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;
  padding: 1rem;
}
.radio{
  display: flex;
  flex-direction: column;
}
.radio-form{
  display: flex;
  flex-direction: column;
}
.radio-title{
  padding: 1rem 0;
  text-transform: capitalize;
}
.radio-form>span{
  padding: 0.5rem 0;
}
.radio-form>span>input{
  margin-right: 1rem;
}

.range-title-box{
  display: flex;
  justify-content: space-between;
}
.range-title-box>span{
  font-size: 1.2rem;
  font-weight: 600;
}
.range-title{
  text-transform: capitalize;
}
.range-form>span>input{
  margin: 1rem 0;
  width: 100%;
}

.check-title{
  padding: 1rem 0;
  text-transform: capitalize;
}
.check-form{
  display: flex;
  justify-content: space-between;
}
.check-form>span{
  padding: 0.5rem 0;
}
.check-form>span>input{
  margin-right: 1rem;
}

</style>