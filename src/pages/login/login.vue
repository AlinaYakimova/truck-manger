<template lang="pug">
.login-page-component
  h1.title ВХОД
  form.form
    .form-rows
      .form-row.form-row--modified
        app-input(
          placeholder="телефон"
        )
      .form-row.form-row--modified
        app-input(
          placeholder="пароль"
        )
      .form-row.form-row--modified
        .form-btn
          app-button(
            title="получить код"
          )
      .form-row
        app-input(
          placeholder="код подтверждения"
        )
    .form-buttons
      .form-btn.form-btn--modified
        app-button(
          title="войти"
        )
      .form-btn.form-btn--modified
        app-button(
          plain
          title="регистрация"
        )
      .form-btn
        app-button(
          plain
          title="забыл пароль"
        )
</template>

<script>

import appInput from "../../components/input";
import appButton from "../../components/button";

export default {
  components: {
    appInput,
    appButton
  },
  data () {
    return {
      
    }
  }
}
</script>

<style lang="scss" scoped src="./login.scss">
  
</style>