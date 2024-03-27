<template>
  <div class="plans">
    <h1 class="plans__header">Выберите тариф для вашего бизнеса</h1>

    <div class="plans__list">
      <PlanCard :item="plansList[0]"/>
      <PlanPrimaryCard :item="plansList[1]"/>
      <PlanCard :item="plansList[2]"/>
    </div>
  </div>
</template>

<script setup>
import PlanCard from "../PlanCard.vue";
import PlanPrimaryCard from "../PlanPrimaryCard.vue";
import {plansList} from "../../services/db.js";
</script>