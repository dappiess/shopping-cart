<template>
  <div id="app">
    <ViewHeader/>
    <div class="container">
      <div class="row">
        <div class="col-8">
          <ProductList/>
        </div>  
        <div class="col-4">
          <ViewCart />
        </div>
      </div>
    
    </div>
  </div>
</template>

<script>
import ViewHeader from './components/ViewHeader';
import ProductList from './components/ProductList.vue'
import ViewCart from './components/ViewCart';

export default {
  name: 'App',
  components:{
  ViewHeader,
  ProductList,
  ViewCart,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
