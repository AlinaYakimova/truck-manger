<template lang="pug">
.foreign_passport-page-component
  .user-avatar
    avatar(
      size="4"
      :src="userPic"
      name="Имя"
      surname="Фамилия"
    )
  h1.title ПАСПОРТ ДЛЯ ВЫЕЗДА ЗА ГРАНИЦУ
  form.form
    .form-rows
      .form-row
        app-input(
          placeholder="серия, номер"
        )
      .form-row
        app-input(
          placeholder="дата выдачи"
        )
      .form-row
        app-input(
          placeholder="дата окончания срока"
        )
      .form-row
        app-input(
          placeholder="орган, выдавший документ"
        )
      .form-row
        app-button(
          title="+ ВТОРОЙ ПАСПОРТ ДЛЯ ВЫЕЗДА"
        )
    .form-buttons
      .form-btns
        .form-btn.form-btn--modified
          app-button(
            title="ВЫХОД"
            grey
          )
        .form-btn.form-btn--modified
          app-button(
            title="ДАЛЕЕ"
          )
      .form-btn
        app-button(
          title="сохранить"
        )
</template>

<script>

import appInput from "../../components/input";
import appButton from "../../components/button";
import avatar from "../../components/avatar";

export default {
  props: {  
    src: String,
  },
  components: {
    appInput,
    appButton,
    avatar
  },
  computed: {
    userPic() {
       return "https://picsum.photos/300/300";
    },
  },
}
</script>

<style lang="scss" scoped src="./foreign_passport.scss">

</style>