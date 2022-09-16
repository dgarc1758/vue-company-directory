<script setup>
    import { faker } from '@faker-js/faker'
</script>


<template>
    <img :src="faker.internet.avatar" alt="" srcset="" />
        <span class=" ">{{ faker.name.fullName()}}</span>
    
</template>