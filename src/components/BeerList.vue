<template>
<div>
    <!-- <ul>
    <li v-for="beer in allBrewDogBeers"> {{ beer.name }}</li>
</ul> -->
    <beer v-for="(beer, index) in all-beers" :key="index" v-bind:beer="beer"></beer>

</div>
</template>

<script>
import Beer from "./Beer.vue";

export default {
    name: "beer-list",
    data() {
        return {};
    },
    props: ["all-beers"],
    components: {
        beer: Beer,
    },
};
</script>

<style scoped></style>
