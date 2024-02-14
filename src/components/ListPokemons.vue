<script setup>
const pokemon = defineProps(["name","urlBaseSvg"])
</script>

<template>
    <div class="col-4">
      <div class="card p-2 mb-3 cardListPokemon">
        <p class="text-center"> {{ pokemon.name }} </p>
        <img :src="urlBaseSvg" class="card-img-top" alt="..."
        height="80"
        />
    </div>


</div>



</template>

<style scoped>
.cardListPokemon{
  background: rgb(70,217,252);
background: radial-gradient(circle, rgba(70,217,252,0.5031550480769231) 21%, rgba(72,63,251,1) 100%);
cursor: pointer;
}
.cardListPokemon:hover {
  background: rgb(70,108,252);
background: radial-gradient(circle, rgba(70,108,252,0.5031550480769231) 21%, rgba(72,63,251,1) 100%);
}
.cardListPokemon img:hover{
  padding: .1rem;
}

</style>