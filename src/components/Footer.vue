<template>
  <div class="container-fluid px-0 mx-0 footer pt-5 pb-4 w-100">
    <div class="row mx-0">
      <div class="col-12">
        <img src="../assets/logo.png" class="logo" alt="">
        <p class="logo-text mb-5">Insights & Innovation Agency</p>

        <p class="footer-text">&copy; {{currentYear}} Phosphene | All rights reserved.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer',
  data() {
    return {
      currentYear: new Date().getFullYear()
    }
  }
}
</script>

<style lang="scss">
.logo {
  height: 50px;
}
.logo-text {
  font-family: SourceRegular;
  font-size: 20px;
  margin-top: -5px;
}

.footer-text {
  font-family: SourceRegular;
  font-size: 17px;
}

.footer {
  background-color: #f2f2f2;
}
</style>
