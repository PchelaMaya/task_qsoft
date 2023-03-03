<script setup>
import { reactive } from 'vue'

import './mob.scss'
const partners = reactive({
    title: 'Наши партнеры',
    companies: [
        {
            id: 0,
            img: 'src/assets/Partners-img/henkel.png',
            img_sr: 'src/assets/Partners-img/henkel-sr.png',
            img_min: 'src/assets/Partners-img/henkel-min.png',
        },
        {
            id: 1,
            img: 'src/assets/Partners-img/john_deere.png',
            img_sr: 'src/assets/Partners-img/john_deere-sr.png',
            img_min: 'src/assets/Partners-img/john_deere-min.png',
        },
        {
            id: 2,
            img: 'src/assets/Partners-img/mcdonalds.png',
            img_sr: 'src/assets/Partners-img/mcdonalds-sr.png',
            img_min: 'src/assets/Partners-img/mcdonalds-min.png',
        },
        {
            id: 3,
            img: 'src/assets/Partners-img/ikea.png',
            img_sr: 'src/assets/Partners-img/ikea-sr.png',
            img_min: 'src/assets/Partners-img/ikea-min.png',
        },
        {
            id: 4,
            img: 'src/assets/Partners-img/reebok.png',
            img_sr: 'src/assets/Partners-img/reebok-sr.png',
            img_min: 'src/assets/Partners-img/reebok-min.png',
        },
        {
            id: 5,
            img: 'src/assets/Partners-img/nike.png',
            img_sr: 'src/assets/Partners-img/nike-sr.png',
            img_min: 'src/assets/Partners-img/nike-min.png',
        },
        {
            id: 6,
            img: 'src/assets/Partners-img/caterpilar.png',
            img_sr: 'src/assets/Partners-img/caterpilar-sr.png',
            img_min: 'src/assets/Partners-img/caterpilar-min.png',
        },
    ]
})
</script>
<template>
<section class="partners w-inner">
    <h2 class="partners__title">{{partners.title}}</h2>
    <div class="partners__content">
        <div class="partners__companies" 
            v-for="company in partners.companies"
        >
            <a class="partners__companies--item"
                :href="'/companies/' + company.id"
            >
                <img class="partners__companies--item--img partners__companies--item--img-max"
                    :src='company.img'
                    alt="company"
                >
                <img class="partners__companies--item--img partners__companies--item--img-sr"
                    :src='company.img_sr'
                    alt="company"
                >
                <img class="partners__companies--item--img partners__companies--item--img-min"
                    :src='company.img_min'
                    alt="company"
                >
            </a>
        </div>
    </div>
</section>
</template>