<template>
<div class="temps">
  <label for="profession2"> Couleur : </label>
  <select name="select-profession2" id="select-profession2">
    <option value="Lycéen"> Modèle DS </option>
    <option value="Employé"> Modèle CS </option>
  </select>
 

 </div>

</template>

<script>



export default {
  
  name: 'MenuSelect',
  props: {
    msg: String
  },
  data () {
      
      return {
        


  
    }
    }
};

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
p{
    margin-top: 40px;
}

</style>

