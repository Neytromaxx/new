<template >
    <ul class="movie-list list-group">
        <movie-list-item v-for="movie in movies" :movie="movie" :key="movie"></movie-list-item>
    </ul>
</template>
<script setup>
import { ref } from 'vue';
import MovieListItem from '../movie-list-item/MovieListItem.vue';

const movies = ref([
    {
        name: 'Omar',
        viewer: 811
    },
    {
        name: 'Ertugrul',
        viewer: 111
    },
    {
        name: 'The empire',
        viewer: 911
    }
])
</script>
<style scoped>
    .movie-list{
        margin-top: 2rem;
        padding: 1.5rem;
        background-color: #fcfaf5;
        border-radius: 4px;
        box-shadow: 15px 15px 15px rgba(0, 0, 0, .15);
    }
</style>