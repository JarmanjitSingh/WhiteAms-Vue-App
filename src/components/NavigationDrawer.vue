<script setup>
import { useRouter } from 'vue-router';
import { useDrawerStore } from "../stores/counter"

const store = useDrawerStore();

const router = useRouter()

function navigateDasboard() {
    router.push({ path: '/' })
}
function navigatePolicies() {
    router.push({ path: '/policies' })
}
function navigateLeads() {
    router.push({ path: "/leads" })
}
function navigateContacts() {
    router.push({ path: '/contacts' })
}
</script>


<template>
    <v-navigation-drawer expand-on-hover rail v-model="store.drawer">

        <v-list>
            <v-list-item prepend-avatar="src/assets/jarman.jpg" title="Jarmanjit Singh"
                subtitle="jarmanjits176@gmail.com"></v-list-item>
        </v-list>

        <v-divider></v-divider>

        <v-list density="compact" nav>
            <v-list-item prepend-icon="mdi-home-account" title="Dashboard" value="dashboard" color="yellow-darken-2"
                @click="navigateDasboard"></v-list-item>
            <v-list-item prepend-icon="mdi-shield" title="Policies" value="policies" color="blue-darken-2"
                @click="navigatePolicies"></v-list-item>
            <v-list-item prepend-icon="mdi-account-multiple" title="Leads" value="leads" color="green-darken-2"
                @click="navigateLeads"></v-list-item>
            <v-list-item prepend-icon="mdi-contacts" title="Contacts" value="contacts" color="purple-darken-2"
                @click="navigateContacts"></v-list-item>
        </v-list>

    </v-navigation-drawer>
</template>

<style scoped></style>