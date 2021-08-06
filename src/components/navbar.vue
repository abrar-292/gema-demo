<template>

</template>

<script>
export default {
  name: 'NavBar',
}
</script>

<style scoped lang="scss">
.nav-item {
  a {
    color: #484848;
    font-family: RobotoFontsBold;
    font-size: 15px;
    margin-right: 20px;
}

  .login-btn {
    width: 100px;
    border: 1px solid #50c9bc;
    border-radius: 3px !important;
    background: transparent;
    color: #50c9bc;
    font-size: 15px;
    line-height: 30px;
    font-family: RobotoFontsBold;
    height: 42px;
    margin-right: 20px;
}

  .sign-up-btn {
    //width: 100px;
    border: 1px solid #FF5252;
    border-radius: 3px !important;
    background: #FF5252;
    color: #ffffff;
    font-size: 15px;
    line-height: 30px;
    font-family: RobotoFontsBold;
    height: 42px;
}

  .login-btn-example {
    width: 120px;
    border: 1px solid #006199;
    border-radius: 3px !important;
    background: transparent;
    color: #006199;
    line-height: 30px;
    font-size: 15px;
    font-family: RobotoFontsBold;
    height: 42px;
    margin-right: 35px;
}

  .sign-up-btn-example {
    //width: 120px;
    border: 1px solid #006199;
    border-radius: 3px !important;
    background: #006199;
    color: #ffffff;
    font-size: 15px;
    line-height: 30px;
    font-family: RobotoFontsBold;
    height: 42px;
}

  .feature-text {
    color: #ffffff;
}
}

.navbar-nav {
  li.active {
    a {
      color: #50c9bc !important;
  }
}
}

.nav-change {
  li.active {
    a {
      color: #50c9bc !important;
  }
}
}

.nav-change {
  .active-change.active {
    a {
      color: #50c9bc !important;
  }
}
}

@media screen and (min-width: 320px) and (max-width: 991px) {
.nav-item {
  display: contents !important;
}
}

.navbar-toggler {
  color: rgba(0, 0, 0, .5);
  border-color: rgba(0, 0, 0, .1);

  &:focus {
    outline: none;
}
}

.navbar-toggler-icon {
  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='30' height='30' viewBox='0 0 30 30'%3e%3cpath stroke='rgba(0, 0, 0, 0.5)' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");
}

</style>
