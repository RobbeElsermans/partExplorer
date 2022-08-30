<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <div class="columns">
      <div class="column">
        <p>blabla</p>
      </div>
      <div class="column">
        <table class="table">
          <tr>
            <th>NAME</th>
            <th>VALUE</th>
            <th>TYPE</th>
            <th>PACKAGE</th>
            <th>QUANTITY</th>
            <th>WEBSITE</th>
            <th>COMMENT</th>
            <th>FOOTPRINT</th>
            <th>DATASHEET</th>
          </tr>
          <tr v-for="(item, i) in database" v-bind:key="i">
            <th v-for="(cell, i) in item" v-bind:key="i">{{ cell }}</th>
          </tr>
        </table>
      </div>
    </div>

  </div>
</template>

<script>
// @ is an alias to /src

export default {
  /* eslint-disable */
  name: 'HomeView',
  data() {
    return {
      database: [
        ["M3", "M3", "M3", "M3", "M3", "M3", "M3", "M3", "M3"],
        ["M5", "M5", "M5", "M5", "M5", "M5", "M5", "M5", "M5"],
        ["M8", "M8", "M8", "M8", "M8", "M8", "M8", "M8", "M8"]
      ]
    }
  },
  methods: {
    getData(id){
      if(id == -1){
        //Get all data

      }
      else
      {
        //get specific data
        
      }
    }
  }
}
</script>

<style>
tr {
  border-width: 2px;
  border-color: black;
  border-style: solid;
}
</style>