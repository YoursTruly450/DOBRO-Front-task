<template>
  <div>
    <section class="order__section">
      <order-water class="water" @get-total-cost="getTotalCost"></order-water>
      <order-time class="time"></order-time>
    </section>
    <total-cost :totalCost="totalCost" class="total"></total-cost>
  </div>
</template>

<script>

import OrderWater from './orderWater.vue';
import OrderTime from './orderTime.vue';
import TotalCost from './totalCost.vue';

export default {
  name: 'Order',
  components: {
    OrderWater, OrderTime, TotalCost,
  },
  props: {},
  data() {
    return {
      totalCost: 0,
    };
  },
  computed: {
  },
  created() {
  },
  mounted() {},
  methods: {
    getTotalCost(data) {
      this.totalCost = data.data;
    },
  },
  watch: {},
};
</script>