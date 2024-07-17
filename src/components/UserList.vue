<template>
<div>
<h1>User List</h1>
<ul>
<li v-for="user in users" :key="user.id">
    {{ user.firstName}}
    {{ user.lastName}}
    {{ user.email}}
</ul>
</div>
</template>

<script lang="ts">
import {defineComponent, ref, onMounted } from 'vue';
import axios from 'axios';

interface User {
    id: number;
    firstName: string;
    lastName: string;
    email: string;
}

</script>