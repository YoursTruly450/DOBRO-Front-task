<template>
    <div>
        <section class="order__section">
            <order-water class="water"></order-water>
            <order-time class="time"></order-time>
        </section>
        <total-cost></total-cost>
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
        return {};
    },
    computed: {
    },
    created() {
    },
    mounted() {},
    methods: {
    },
    watch: {},
};
</script>