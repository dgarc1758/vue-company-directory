<script setup>
import { faker } from '@faker-js/faker'
const firstName = faker.name.firstName()
const lastName = faker.name.lastName()
const fullName = `${firstName} ${lastName}`

const selectCard = () => {
    console.log(`${fullName} selected`)
}
</script>


<template>
    <div class="card" @click="selectCard">
     <div class="card-image">
        <img :src="faker.internet.avatar" alt="" srcset="" />
     </div>
     <div class="card-details">
            <p class="card-details-name">{{ fullName}}</p>
            <p class="card-details-job">{{ faker.name.jobTitle()}},{{faker.name.jobArea()}}</p>
            <p class="card-details-email">{{ faker.internet.exampleEmail(firstName, lastName)}}</p>
            <p class="card-details-quote">{{faker.lorem.paragraph()}}</p>
      </div>  
    </div>
</template>

<style scoped lang="postcss">
    .card{
        @apply cursor-pointer overflow-hidden rounded-md bg-slate-100 p-8 shadow-md transition-transform duration-300 hover:scale-110 hover:shadow-2xl hover:shadow-slate-900;
    }

</style>