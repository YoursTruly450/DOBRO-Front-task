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
          isTotalCost: null,
          isName: null,
          isPhone: null,
          isMail: null,
          isAdress: null,
          isCheckedPersonalData: null,
          isDateDay: null,
          isDateTime: null,
        };
    },
    computed: {
    },
    created() {
    },
    mounted() {},
    methods: {
      getContacts(data) {
        this.isName = data.isName;
        this.isMail = data.isMail;
        this.isPhone = data.isPhone;
        this.isAdress = data.isAdress;
        this.isChecked = data.isChecked;
      },
      submitOrder(){},
    },
    watch: {},
};
</script>