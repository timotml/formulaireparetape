<template>

      <section>
  <h3>Sexe :</h3>
  <input type="radio" v-model="color" value="0">Masculin
  <input type="radio" v-model="color" value="1">Féminin
  
  <br />
 
</section>

</template>

<script>

export default {
  
  name: 'MenuRadio',
  props: {
    msg: String
  },
}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
  display: grid;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}


#start{
  margin-left: 10px;
  margin-top: 30px;
}

</style>

