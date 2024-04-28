<script setup>
//props - onMounted, reactive, ref
import { onMounted, reactive, ref } from 'vue';
import ListCharacters from '../components/ListCharacters.vue';

let characters = reactive(ref())

//fetch - axios
onMounted(() => {
  fetch("https://rickandmortyapi.com/api/character?limit=20%offset=0")
  .then(response => response.json())
  .then(response => {
    characters.value = response.results
    console.log(characters)
  });
})

</script>

<template>
  <main>
    <div class="container">
      <div class="row mt-4">
        <div class="col-sm-12 col-md-12">
          <div class="card rounded-5">
            <div class="card-body row bg-black bg-gradient rounded-5">
              <ListCharacters
            v-for="character in characters"
            :key="character.name"
            :image="character.image"
            :name="character.name"
            :status="character.status"
            :species="character.species"
            :gender="character.gender"
            :location="character.location.name"
            :episode="character.episode"
            />
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
