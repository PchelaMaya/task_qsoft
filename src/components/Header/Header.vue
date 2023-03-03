<script setup>
import "./mob.scss"
import "./desc.scss"
</script>
<template>
    <header class="header">
        <div class="header__inner w-inner">
            <div class="header__top">
                <a class="header__top--logo" href="/">
                    <img src="@/assets/Header-img/logo.png">
                </a>
                <div class="header__search header__search--desc">
                    <button class="header__search--btn">
                        <img src="@/assets/Header-img/search.png">
                    </button>
                    <input class="header__search--input" type="text" placeholder="Найти...">
                </div>
                <a class="header__top--user header__top--user--mobile">
                    <img src="@/assets/Header-img/avatar.png">
                </a>
                <a class="header__top--user header__top--user--desc">
                    <p class="header__top--user--name">Константин</p>
                    <img src="@/assets/Header-img/avatar_desc.png">
                </a>

            </div>
            <div class="header__search header__search--mobile">
                <button class="header__search--btn">
                    <img src="@/assets/Header-img/search.png">
                </button>
                <input class="header__search--input" type="text" placeholder="Найти...">
            </div>
        </div>
    </header>
</template>