<script setup>
import "./mob.scss"
</script>
<template>
    <header class="header">
        <div class="header__inner w-inner">
            <div class="header__top">
                <a class="header__top--logo" href="/">
                    <img src="@/assets/Header-img/logo.png">
                </a>
                <a class="header__top--avatar">
                    <img src="@/assets/Header-img/avatar.png">
                </a>
            </div>
            <div class="header__search">
                <button class="header__search--btn">
                    <img src="@/assets/Header-img/search.png">
                </button>
                <input class="header__search--input" type="text" placeholder="Найти...">
            </div>
        </div>
    </header>
</template>