<template>
<div class="prix">
    <h3>Prix : {{value1}}</h3><!--Je cherche à crééer un variable fain que mon prix change en fonctionne de la taille du rail -->
<h4>Etant donné que je n'ai pas réussi a faire le prix, je vous invite a multiplier par 1,5 votre longueur en cm afin de le connaitre</h4>
<h4>Si vous prenez un modele DS, le prix reste inchanger et si vous prenez un CS, vous pouvez multiplier le prix par 1,8</h4>
<h4>Les couleurs n'influencent pas le prix </h4>


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
div{
    background-color: coral;
}
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

