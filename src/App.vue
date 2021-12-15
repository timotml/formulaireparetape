<template>
  <div id="app">
    <img alt="logo" src="./assets/tringles-rail.jpg" height="200" width="200">
     <TextInput msg=""/>
    <TextInput msg=""/> <!--Envoyer une props à un composant -->
    

    

<div v-if="step === 'step1'">
  <h1>Etape:1/3</h1>
  <h3>Entrez votre longueur de rail (min 0cm - max 200cm) : </h3>
  <span>{{ value1 }}</span>
<br>
<input type="text" v-model="message" placeholder="min 0cm - max 200cm">
      <Price msg=""/>
      <Button msg="" v-on:validation="step='step2'"/>
</div>
<div v-if="step === 'step2'">
  <h1>Etape:2/3</h1>
  <br>
  <h3>Selectionner le type : </h3>
   <h4>Modèle DS : Fixation au plafond pour rideaux légers
(sans doublure, hauteur max 300cm)</h4>
<h4>Modèle CS : Fixation au plafond ou au mur pour rideaux lourds
(doublé, hauteur + 300 cm)</h4>
  <MenuSelect2 msg=""/>
      <Price msg=""/>
   
        <Button msg="" v-on:validation="step='step3'" v-on:reinitialiser="step='step1'"/>  
</div>

<div v-if="step === 'step4'">
  <h1>Article Bien ajouté au panier</h1>
  <br>
   <h3>Pour passez au payement Cliquez sur Valider, si vous souhaitez recommencer la personnalisation cliquez sur Reinitialiser </h3>

        <Button msg=""  v-on:reinitialiser="step='step1'"/>  
</div>


<div v-if="step === 'step3'">
  <h1>Etape:3/3</h1>
  <br>
   <h3>Selectionner la couleur : </h3>
    <MenuSelect msg=""/>
        <Price msg=""/>
  <Button msg="" v-on:validation="step='step4'" v-on:reinitialiser="step='step2'"/>
 

</div>
</div> 
</template>

<script>

import TextInput from './components/TextInput.vue';
import MenuSelect from './components/MenuSelect.vue';
import MenuSelect2 from './components/MenuSelect2.vue';
import Button from './components/Button.vue';
import Price from './components/Price.vue';




export default {
  name: 'App',
  components: {
    TextInput,
    MenuSelect,
    MenuSelect2,
    Button,
    Price,
  },
    
data(){
  return{
    colorie :'red',
    step:'step1',
}

}
}

</script>

<style>
#app {
  background-color: rgb(90, 144, 245);
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>
