<script setup>
import myCardVignette from './myCardVignette.vue'
import { reactive } from 'vue'
 
const response = [
    {
        description: 'Description de la card',
        title: "100% Gratuit",
        imageSrc : 'http://placekitten.com/300/150',
        imageAlt : 'Image de chat',
        buttonLabel: "Bouton de la card"
    }, 
    {
        description: 'Description de la card',
        title: "100% ecolo",
        imageSrc : 'http://placekitten.com/300/150',
        imageAlt : 'Image de chat',
        buttonLabel: "Bouton de la card"
    },
    {
        description: 'Description de la card',
        title: "Retours gratuits",
        imageSrc : 'http://placekitten.com/300/150',
        imageAlt : 'Image de chat',
        buttonLabel: "Bouton de la card"
    },
    {
        description: 'Description de la card',
        title: "Retours gratuits",
        imageSrc : 'http://placekitten.com/300/150',
        imageAlt : 'Image de chat',
        buttonLabel: "Bouton de la card"
    },
    {
        description: 'Description de la card',
        title: "Retours gratuits",
        imageSrc : 'http://placekitten.com/300/150',
        imageAlt : 'Image de chat',
        buttonLabel: "Bouton de la card"
    },
    {
        description: 'Description de la card',
        title: "Retours gratuits",
        imageSrc : 'http://placekitten.com/300/150',
        imageAlt : 'Image de chat',
        buttonLabel: "Bouton de la card"
    }
]

const cards = reactive(response)
</script>

<template>
    <div class='cards'>
        <myCardVignette v-for='card in cards' v-bind='card' /> 
    </div>
</template>

<style lang='scss' scoped>
.cards{
  display: grid;
  gap: rem(30);
  grid-template-columns: repeat(3, 1fr);
}
</style>
