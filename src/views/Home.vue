<script setup>
import { storeToRefs } from 'pinia';

import { useAuthStore } from '@/stores';

const authStore = useAuthStore();
const { user } = storeToRefs(authStore);
</script>

<template>
    <div v-if="user">
        <h1>Bienvenido administrado de TUSCORE:  {{user.firstName}}!</h1>
       
        <p><router-link to="/partidos">Partidos</router-link></p>
    </div>
 
</template>
