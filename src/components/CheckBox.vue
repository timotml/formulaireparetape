<template>
<ul>
    <h3>Compétences</h3>
    <li>
        <input id="checkbox1" class="checkbox" type="checkbox">
        <label for="checkbox1">Marketing</label>
    </li>
    <li>
        <input id="checkbox2" class="checkbox" type="checkbox">
        <label for="checkbox2">Communication</label>
    </li>
    <li>
        <input id="checkbox3" class="checkbox" type="checkbox">
        <label for="checkbox3">Design</label>
    </li>
    <li>
        <input id="checkbox4" class="checkbox" type="checkbox">
        <label for="checkbox4">Developpeur</label>
    </li>

</ul>
</template>

<script>
export default {
  
  name: 'Checkbox',
  props: {
    msg: String,
  },
}
</script>

<style scoped>
h3{
    margin: 30px 0 0;
}
ul{
    list-style-type: none;
    padding: 0;
    display: grid;

}
li{
    display:inline-block;
}
a{
    color: aqua;
}

</style>