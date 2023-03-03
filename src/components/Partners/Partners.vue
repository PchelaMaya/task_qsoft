<script setup>
import { reactive } from 'vue'

import './mob.scss'
const partners = reactive({
    title: 'Наши партнеры',
    companies: [
        {
            id: 0,
            img: 'src/assets/Partners-img/henkel.png'
        },
        {
            id: 1,
            img: 'src/assets/Partners-img/john_deere.png'
        },
        {
            id: 2,
            img: 'src/assets/Partners-img/mcdonalds.png'
        },
        {
            id: 3,
            img: 'src/assets/Partners-img/ikea.png'
        },
        {
            id: 4,
            img: 'src/assets/Partners-img/reebok.png'
        },
        {
            id: 5,
            img: 'src/assets/Partners-img/nike.png'
        },
        {
            id: 6,
            img: 'src/assets/Partners-img/caterpilar.png'
        },
    ]
})
</script>
<template>
<section class="partners w-inner">
    <h2 class="partners__title">{{partners.title}}</h2>
    <div class="partners__companies" 
        v-for="company in partners.companies"
    >
        <a class="partners__companies--item"
            :href="'/companies/' + company.id"
        >
            <img class="partners__companies--item--img"
                :src='company.img'
                alt="company"
            >
        </a>
    </div>
</section>
</template>