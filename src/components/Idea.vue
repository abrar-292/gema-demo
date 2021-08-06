<template>
  <div class="main-header container mt-5">
    <div class="row mx-0">

      <div class="col-12 what-we-do-div mb-3">
        <h2>IDEAS</h2>
      </div>
      <div class="col-md-6 mb-4" v-for="(item) in items" v-bind:key="item.image">
        <div class="row mx-0 px-0 items-div d-flex align-items-center justify-content-start text-start">
          <div class="col-12">
            <img v-bind:src="require(`../assets/${item.image}`)" class="img-fluid" :alt="item.image">
          </div>
          <div class="texts col-12 mt-3">
            <h3 class="mb-1">{{ item.title }}</h3>
            <p class="mb-1 text-muted">{{ item.text }}</p>
          </div>
        </div>
      </div>

      <div class="col-12 right">
        <button class="btn know-btn">More Ideas</button>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Idea',
  data() {
    return {
      items: [
        {
          image: 'd1.jpg',
          title: 'Do you know what phosphense area?',
          text: '05 November 2017'
        },
        {
          image: 'd2.jpg',
          title: 'Here we are! This is our first post.',
          text: '12 October 2017'
        },
      ]
    }
  }
}
</script>

<style scoped lang="scss">
.main-div {
  text-align: left;

  p {
    font-family: SourceRegular;
    color: #333333;
    font-size: 24px;
    margin: 60px 0;
  }
}

.right {
  text-align: right;
}

.know-btn {
  padding: 5px 40px;
  border-radius: 10px;
  background-color: #50c875;
  color: white;
  font-family: SourceRegular;
  font-size: 25px;
  margin: 0 0 30px 0;
}

.what-we-do-div {
  text-align: left;

  h2 {
    font-family: SourceBold;
    font-size: 40px;
    color: #333333;
  }
}

.items-div {

  .texts {
    h3 {
      font-size: 30px;
      font-family: SourceBold;
    }
    p {
      font-size: 20px;
      font-family: SourceRegular;
    }
  }
}
</style>
