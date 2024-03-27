<template>
  <div class="plancard pro">
    <div class="plancard__header">
      <p class="plancard__title">{{ item.title }}</p>
      <p class="plancard__price"><span class="plancard__num">{{ item.price }}</span>{{ item.currency }}</p>
      <p class="plancard__description">{{ item.description }}</p>
    </div>

    <div class="plancard__body">
      <p class="plancard__advantage">Особенности</p>

      <div class="advantages">
        <div class="advantages__pros" v-for="(pros, ind) in item.features.pros" :key="ind">
          <img class="advantages__icon" src="" alt="">
          <p class="advantages__title">{{ pros }}</p>
        </div>
      </div>

      <div class="advantages">
        <div class="advantages__cons" v-for="(cons, ind) in item.features.cons" :key="ind">
          <img class="advantages__icon" src="" alt="">
          <p class="advantages__title">{{ cons }}</p>
        </div>
      </div>
    </div>

    <div class="plancard__footer">
      <button class="plancard__btn pro__btn">Выбрать</button>
    </div>
  </div>
</template>

<script setup>
defineProps({
  item: Object
})
</script>