<template>
    <div>
      <contacts class="contacts"></contacts>
      <order class="order"></order>
    </div>
</template>

<script>

import Order from './order.vue';
import Contacts from './contacts.vue';

export default {
    name: 'FormSelector',
    components: {
      Order, Contacts,
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