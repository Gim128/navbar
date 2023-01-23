<template>
  <div class="bg-white py-24 sm:py-32 lg:py-24"> 
    <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="sm:text-center">
            <h2 class="text-lg font-semibold leading-8 text-indigo-700">Know About CNT</h2>
            <p class="mt-2 text-2xl font-bold tracking-tight text-gray-900 sm:text-4xl">Why Choose CNT</p>
            <p class="mx-auto mt-6 max-w-2xl text-lg leading-8 text-gray-600">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio veritatis earum, perspiciatis voluptate minus magnam iusto assumenda iste quod consequatur sapiente laudantium suscipit dolores quasi? Possimus non minus quia omnis?
            </p>
        </div>

        <div class="mt-20 max-w-lg sm:mx-auto md:max-w-none">
            <div class="grid grid-cols-1 gap-y-16 md:grid-cols-2 md:gap-x-12 md:gap-y-16">
                <div v-for="feature in features" :key="feature.name" class="realtive flex flex-col gap-6 sm:flex-row md:flex-col lg:flex-row">
                    <div class="flex h-12 w-12 items-center justify-center rounded-xl bg-indigo-600 text-white sm:shrink-0">
                        <component :is="feature.icon" class="h-8 w-8" aria-hidden="true"/>
                    </div>
                    <div class="sm:min-w-0 sm:flex-1">
                        <p class="text-lg font-semibold leading-8 text-gray-900">{{ feature.name }}</p>
                        <p class="mt-2 text-base leading-7 text-gray-600">{{ feature. description }}</p>
                    </div>
                </div>
            </div>
        </div>

    </div>
  </div>
</template>

<script setup>

    const features = [
        {
            name: 'Competative Exchange Rates',
            description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio veritatis earum, perspiciatis voluptate minus magnam iusto assumenda iste quod consequatur sapiente laudantium suscipit dolores quasi? Possimus non minus quia omnis?',
            icon: '',
        },
        {
            name: 'No Hidden Fees',
            description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio veritatis earum, perspiciatis voluptate minus magnam iusto assumenda iste quod consequatur sapiente laudantium suscipit dolores quasi? Possimus non minus quia omnis?',
            icon: '',
        },
        {
            name: 'Transfers are instant',
            description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio veritatis earum, perspiciatis voluptate minus magnam iusto assumenda iste quod consequatur sapiente laudantium suscipit dolores quasi? Possimus non minus quia omnis?',
            icon: '',
        },
        {
            name: 'Mobile Notifications',
            description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio veritatis earum, perspiciatis voluptate minus magnam iusto assumenda iste quod consequatur sapiente laudantium suscipit dolores quasi? Possimus non minus quia omnis?',
            icon: '',
        },
    ]

// export default {
//     name: "FeatureComponent",
// }
</script>

<style>

</style>