<template lang="pug">
.reg-page-component
  h1.title РЕГИСТРАЦИЯ
  form.form
    .form-rows
      .form-row
        app-input(
          placeholder="Фамилия"
        )
      .form-row
        app-input(
          placeholder="Имя"
        )
      .form-row
        app-input(
          placeholder="Отчество"
        )
      .form-row
        app-input(
          placeholder="телефон"
        )
      .form-row
        app-input(
          placeholder="...."
        )
      .form-row
        app-input(
          placeholder="...."
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

export default {
  components: {
    appInput,
    appButton
  }
}
</script>

<style lang="scss" scoped src="./reg.scss">

</style>