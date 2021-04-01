<template>
    <div>
      <h2 class="contacts__header">Заполните данные</h2>
      <section class="contacts__data">
        <input class="contacts__input" type="text" placeholder="Имя">
        <input class="contacts__input" type="text" placeholder="e-mail">
        <input class="contacts__input" type="text" placeholder="Телефон">
        <input class="contacts__input" type="text" placeholder="Адрес">
        <div class="contacts__input-group">
          <input class="contacts__checkbox" type="checkbox">
          <span class="contacts__traitement">Я согласен на 
            <a 
            href="https://ru.wikipedia.org/wiki/%D0%9F%D0%B5%D1%80%D1%81%D0%BE%D0%BD%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5_%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D0%B5">
            обработку персональных данных</a></span>
        </div>
      </section>
    </div>
</template>

<script>

export default {
    name: 'Contacts',
    components: {},
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