<script setup>
    const character = defineProps(["name", "image", "status", "species", "type", "gender", "location", "episode"])
    // const idCharacter = character.url.split('/')[5]
    // const imageUrl = 'https://rickandmortyapi.com/api/character/avatar/' + idCharacter +'.jpeg'
    
</script>

<template>
    <div class="col-md-3">
        <div class="card mb-3 p-2">
            <!-- <img :src="imageUrl" class="card-img-top" width="80" heigth="auto" alt="..."> -->
            <img :src="character.image" class="card-img-top" width="80" heigth="auto" alt="...">
            <div class="card-body">
                <p class="card-title text-center">Nome: {{ character.name }}</p>
                <p class="card-title text-center">Status: {{ character.status }}</p>
                <p class="card-title text-center">Espécie: {{ character.species }}</p>
                <p class="card-title text-center">Gênero: {{ character.gender }}</p>
                <p class="card-title text-center">Localização: {{ character.location }}</p>
                <p class="card-title text-center">Quantidade de Ep: {{ character.episode.length }}</p>
            </div>
        </div>
    </div>
</template>

<style>

</style>