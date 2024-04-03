<template>
  <header class="header">
    <div class="header__logo">
      <div class="logo__wrap">
        <img src="../assets/img/logo.svg" alt="">
        <p>Профильная CRM для турбизнеса</p>
      </div>
      <button class="header__btn">
        <img class="header__burger" src="../assets/img/plus.svg" alt="">
      </button>
    </div>

    <div class="header__swipe">
      <a class="close__btn" href="/#opportunities">Возможности</a>
      <a class="close__btn" href="/#plans">Тариф</a>
      <a class="close__btn" href="/#contacts">Контакты</a>
      <a href="/" class="phone close__btn">+998 (99) 999-99-99</a>

      <button class="lang-switcher">
        <img src="../assets/img/lang/rus.svg" alt="">
        <span>ru</span>
      </button>

      <button class="primary-btn">Записаться <br> на консультацию</button>
      <div class="phone__social">
        <a href=""><img src="../assets/img/dark/facebook.svg" alt=""></a>
        <a href=""><img src="../assets/img/dark/telegram.svg" alt=""></a>
        <a href=""><img src="../assets/img/dark/instagram.svg" alt=""></a>
      </div>
    </div>

    <button class="header__btn">
      <img class="header__burger" src="../assets/img/plus.svg" alt="">
    </button>
  </header>
</template>

<script setup>
import {onMounted} from "vue";

const hideScroll = () => {
  const body = document.querySelector('body');
  body.classList.toggle('lock');
}

onMounted(() => {
  const burgerBtns = document.querySelectorAll('.header__btn');
  const closeBtns = document.querySelectorAll('.close__btn');
  const swipeMenu = document.querySelector('.header');

  function toggleMenu() {
    swipeMenu.classList.toggle('show');
    hideScroll();
  }


  [...burgerBtns, ...closeBtns].forEach(burgerBtn => {
    burgerBtn.addEventListener('click', toggleMenu);
  });
});
</script>
