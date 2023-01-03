<template lang="pug">
.wrapper
  .container
    login
    //- reg
    //- user
    //- passport
    //- driving_license
    //- driver_card
    //- foreign_passport
    //- visa
</template>

<script>

import login from "./pages/login";
import reg from "./pages/reg";
import user from "./pages/user";
import passport from "./pages/passport";
import driving_license from "./pages/driving_license";
import driver_card from "./pages/driver_card";
import foreign_passport from "./pages/foreign_passport";
import visa from "./pages/visa";

export default {
  components: {
    login,
    reg,
    user,
    passport,
    driving_license,
    driver_card,
    foreign_passport,
    visa
  },
  data () {
    return {
      
    }
  }
}
</script>

<style lang="scss">

</style>