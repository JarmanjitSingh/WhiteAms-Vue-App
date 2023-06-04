<script setup>
import { RouterLink } from 'vue-router'
import { useDrawerStore } from "../stores/counter"

const store = useDrawerStore();
</script>

<template>
    <div id="navbar">

        <img src="src/assets/logo3.png" alt="logo" class="logo" />


    </div>

    <v-spacer></v-spacer>

    <v-btn variant="text" icon="mdi-magnify"></v-btn>

<v-btn variant="text" icon="mdi-filter"></v-btn>

<v-btn variant="text" icon="mdi-dots-vertical" @click="store.toggleDrawer"></v-btn>



<!-- <ul>
        <li>
            <RouterLink to="/">Home</RouterLink>
        </li>
        <li>
                    <RouterLink to="/services">Services</RouterLink>
                </li>
                    <li>
                        <RouterLink to="/about">About</RouterLink>
                    </li>
                    <li>
                        <RouterLink to="/contacts">Contacts</RouterLink>
                    </li>
                </ul> -->
</template>

<style scoped>
.logo {
    height: 50px;
    width: 170px;
    object-fit: contain;
    /* border: 2px solid black; */
}
</style>