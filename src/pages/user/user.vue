<template lang="pug">
.user-page-component
  .user-avatar
    avatar(
      size="4"
      :src="userPic"
      name="Имя"
      surname="Фамилия"
    )
  form.form
    .form-rows
      .form-row
        app-input(
          placeholder="дата рождения"
        )
      .form-row
        app-input(
          fieldType="textarea"
          placeholder="адрес\nместа\nжительства"
        )
      .form-row
        app-input(
          placeholder="пол"
        )
      .form-row
        app-input(
          placeholder="должность"
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

<style lang="scss" scoped src="./user.scss">
</style>