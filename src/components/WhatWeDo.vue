<template>
  <div class="main-header container">
    <div class="row mx-0">
      <div class="col-12 main-div">
        <p>
          Phosphene is and independent thinking marketing & research agency. We focus on solving your marketing
          challenges &
          driving your innovation agenda forward using the art and science of human behavioral understanding. you may
          have heard it a
          million times before. and let us say it too - we do not want to be a typical research agency. We do not want
          to follow any established norms.
          We are not blindly after digital platform or neuroscience just because they are breakthroughs and fascinating
          conversation pieces.
          If there is one thing we chase vehemently here, it is pure common sense.
        </p>
      </div>

      <div class="col-12 right">
        <button class="btn know-btn">Know More</button>
      </div>

      <div class="col-12 what-we-do-div mb-3">
        <h2>WHAT WE DO</h2>
      </div>
      <div class="col-12 mb-4" v-for="(item, index) in items" v-bind:key="item.image">
        <div class="row mx-0 px-0 items-div d-flex align-items-center justify-content-start text-start"
             v-bind:class="{ 'text-end': index % 2 !== 0 }">
          <div class="w-auto h-auto px-0" v-if="index % 2 === 0">
            <img v-bind:src="require(`../assets/${item.image}`)" :alt="item.image">
          </div>
          <div class="texts">
            <h3 class="mb-1">{{ item.title }}</h3>
            <p class="mb-1">{{ item.text }}</p>
          </div>
          <div class="w-auto h-auto px-0" v-if="index % 2 !== 0">
            <img v-bind:src="require(`../assets/${item.image}`)" :alt="item.image">
          </div>
        </div>
      </div>

      <div class="col-12 what-we-do-div mb-3 mt-5">
        <h2>ENDORSEMENTS</h2>
      </div>
    </div>
  </div>
  <div class="container-fluid px-0 mx-0 carousel-bg w-100">
    <div class="row mx-auto container pt-5">
      <div class="col-12 py-5">
        <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
          <div class="carousel-inner row mx-0 px-0">
            <div class="carousel-item active">
              <div class="d-flex justify-content-start align-items-center">
                <img class="carousel-img" height="100" width="100" src="../assets/Temp_Profile_Pic1.jpg"
                     alt="Second slide">
                <div class="carousel-text text-start ml-3">
                  <p>"We were truly fortunate to discover Phospene. It has been a very fruitful association for our
                    organization. Highly recommended."</p>
                  <span>Peter Ross, Figel Corp</span>
                </div>
              </div>
            </div>
            <div class="carousel-item">
              <div class="d-flex justify-content-start align-items-center">
                <img class="carousel-img" height="100" width="100" src="../assets/Temp_Profile_Pic1.jpg"
                     alt="Second slide">
                <div class="carousel-text text-start ml-3">
                  <p>"We were truly fortunate to discover Phospene. It has been a very fruitful association for our
                    organization. Highly recommended."</p>
                  <span>Peter Ross, Figel Corp</span>
                </div>
              </div>
            </div>
            <div class="carousel-item">
              <div class="d-flex justify-content-start align-items-center">
                <img class="carousel-img" height="100" width="100" src="../assets/Temp_Profile_Pic1.jpg"
                     alt="Second slide">
                <div class="carousel-text text-start ml-3">
                  <p>"We were truly fortunate to discover Phospene. It has been a very fruitful association for our
                    organization. Highly recommended."</p>
                  <span>Peter Ross, Figel Corp</span>
                </div>
              </div>
            </div>
            <div class="carousel-item">
              <div class="d-flex justify-content-start align-items-center">
                <img class="carousel-img" height="100" width="100" src="../assets/Temp_Profile_Pic1.jpg"
                     alt="Second slide">
                <div class="carousel-text text-start ml-3">
                  <p>"We were truly fortunate to discover Phospene. It has been a very fruitful association for our
                    organization. Highly recommended."</p>
                  <span>Peter Ross, Figel Corp</span>
                </div>
              </div>
            </div>
          </div>
          <ol class="carousel-indicators">
            <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
          </ol>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'WhatWeDo',
  components: {},
  data() {
    return {
      items: [
        {
          image: 'Temp01.jpg',
          title: 'Marketing Research',
          text: 'We can lap up your business challenges and identify ways market research techniques can be a solution. We find your insight, whatever its qualitative or quantitative, online or offline. Ends matter a lot more.'
        },
        {
          image: 'Temp07.jpg',
          title: 'Marketing Research',
          text: 'We can lap up your business challenges and identify ways market research techniques can be a solution. We find your insight, whatever its qualitative or quantitative, online or offline. Ends matter a lot more.'
        },
        {
          image: 'Temp03.jpg',
          title: 'Marketing Research',
          text: 'We can lap up your business challenges and identify ways market research techniques can be a solution. We find your insight, whatever its qualitative or quantitative, online or offline. Ends matter a lot more.'
        },
        {
          image: 'Temp04.jpg',
          title: 'Marketing Research',
          text: 'We can lap up your business challenges and identify ways market research techniques can be a solution. We find your insight, whatever its qualitative or quantitative, online or offline. Ends matter a lot more.'
        },
      ],
      carouselItems: [
        {
          image: 'Temp_Profile_Pic1.jpg',
          name: 'Peter Ross, Figel Corp',
          text: '"We were truly fortunate to discover Phospene. It has been a very fruitful association for our organization. Highly recommended."'
        },
        {
          image: 'Temp_Profile_Pic1.jpg',
          name: 'Peter Ross, Figel Corp',
          text: '"We were truly fortunate to discover Phospene. It has been a very fruitful association for our organization. Highly recommended."'
        },
        {
          image: 'Temp_Profile_Pic1.jpg',
          name: 'Peter Ross, Figel Corp',
          text: '"We were truly fortunate to discover Phospene. It has been a very fruitful association for our organization. Highly recommended."'
        },
        {
          image: 'Temp_Profile_Pic1.jpg',
          name: 'Peter Ross, Figel Corp',
          text: '"We were truly fortunate to discover Phospene. It has been a very fruitful association for our organization. Highly recommended."'
        },
      ],
    }
  },
  methods: {}
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
  background-color: #f2f2f2;

  img {
    height: 175px;
    width: 175px;
  }

  .texts {
    width: calc(100% - 175px);

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

.carousel-bg {
  background-color: #f2f2f2;
}

.carousel-indicators {
  height: 30px;
  position: relative !important;
  bottom: -50px;

  li.active {
    background-color: #50c875;
  }

  li {
    height: 15px;
    width: 15px;
    background-color: #c8c8c8;
    margin: 0 10px;
    border-radius: 50%;
    cursor: pointer;
  }
}

.carousel-img {
  height: 175px;
  width: 175px;
  margin-right: 20px;
}

.carousel-text {
  p {
    font-size: 24px;
    text-align: left;
    font-family: SourceRegular;
  }

  span {
    font-size: 24px;
    text-align: left;
    font-family: SourceItalic;
  }
}
</style>
