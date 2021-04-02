<template>
    <div>
      <contacts class="contacts" @get-contacts="getContacts"></contacts>
      <order class="order"></order>
      <section class="submit">
        <input type="submit" @click="submitOrder" class="submit__input" value="Заказать воду">
      </section>
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
        return {
          totalCost: 0,
          name: '',
          phone: '',
          mail: '',
          adress: '',
          isCheckedPersonalData: null,
          dateDay: '',
          dateTime: '',
        };
    },
    computed: {
      isChecked() {
        if (this.isCheckedPersonalData) {
          return true;
        } else {
          return false;
        }
      }
    },
    created() {
    },
    mounted() {},
    methods: {
      getContacts(data) {
        console.log(data);
      },
      submitOrder(){},
    },
    watch: {},
};
</script>