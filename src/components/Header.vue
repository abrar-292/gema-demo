<template>
  <div class="main-header">
    <div class="row mx-0">
      <div class="col-md-3 main-div">
        <div class="d-flex justify-content-center">
          <h1>
            We are an
            <span>Insight &</span>
            <span>Innovation</span>
            Agency
          </h1>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style scoped lang="scss">
.main-header {
  background: url('../assets/Temp_Hero123.jpg') no-repeat 100% 100%;
  background-size: cover;

  .main-div {
    background-color: #00000061;
    padding: 150px 15px;
    text-align: left;

    h1 {
      font-family: SourceRegular;
      color: white;

      span {
        font-family: SourceBold;
        display: block;
      }
    }
  }
}
</style>
