<template>
  <div id="app">

    <nav class="nav nav-bar">

      <ul class="nav">
        <li class="nav-item"><router-link class="nav-link" to="/">Home</router-link></li>
        <li class="nav-item"><router-link class="nav-link" to="/users/10">Users 10</router-link></li>
        <li class="nav-item"><router-link class="nav-link" to="/users/12">Users 12</router-link></li>
      </ul>
    </nav>
   
    <hr>
      <div class="container-fluid">
          <div class="jumbotron">
       <h1>Experiment with Vue Router</h1>
    </div>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-md-6">
          <router-view></router-view>
        </div>
        <div class="col-md-6">
          <app-message></app-message>
        </div>
      </div>
          
         
    </div>

  </div>
</template>

<script>
export default {
  data () {
    return {
     
    }
  }
}
</script>

<style>

  *{
    font-family: sans-serif;
  }

</style>
