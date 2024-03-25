<template>
  <div class="offered">
    <h1 class="offered__header">Предлагаемые услуги</h1>
    <p class="offered__description">
      Предлагаем вам широкий спектр услуг чтобы помочь вам
      эффективно управлять вашим бизнесом.
    </p>

    <div class="offered__list">
      <div class="service" v-for="el in services" :key="el.id">
        <div class="service__left">
          <img :src="el.img" alt="">
        </div>
        <div class="service__right">
          <div class="service__wrap">
            <h1 class="service__header">{{ el.title }}</h1>
            <p class="service__description">{{ el.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import firstImg from '../assets/img/offered/first.png'
import secondImg from '../assets/img/offered/second.png'
import thirdImg from '../assets/img/offered/third.png'

const services = [
  {
    id: 1,
    title: 'Клиентская база',
    img: firstImg,
    description: 'Клиентская база в CRM-системе представляет собой ценный актив для\n' +
        'бизнеса, который может принести ряд преимуществ. Она позволяет \n' +
        'отслеживать и управлять воронкой продаж, анализировать данные о \n' +
        'потенциальных клиентах, прогнозировать продажи и многое другое.'
  },
  {
    id: 2,
    title: 'Продажа и касса',
    img: secondImg,
    description: 'Система предоставляет обширный функционал для учета финансов и \n' +
        'финансовых операций:\n' +
        '- Кассовая книга для учета финансов компании.\n' +
        '- Автоматическая синхронизация курсов валют туроператоров и \n' +
        '  автоматический пересчет долга при изменении курса туроператора, \n' +
        '  а также множество других возможностей.'
  },
  {
    id: 3,
    title: 'Интеграции и возможности',
    img: thirdImg,
    description: '- Интеграция с сервисом создания подборок Qui-Quo.\n' +
        '- Интеграция с облачной и офисной IP-телефонией.\n' +
        '- Быстрый логин. Специальное расширение для автоматического \n' +
        'заполнения логина и пароля.\n' +
        '- Массовые и индивидуальные SMS-рассылки.\n' +
        '- Авто-заполнение документов по сканированию паспорта.\n' +
        '- История Действия и множество других возможностей.'
  },

]
</script>