<template>
<div class="buttons">
      
     <button v-on:click="$emit('validation')">Validation</button>
     <button v-on:click="$emit('reinitialiser')">Réinitialiser</button>

      </div>
</template>

<script>

export default {
      name: "Button",
      props: {
            msg: String,
      },
      data(){
            return
        
      }
}

  


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>

