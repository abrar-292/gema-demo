<template>
  <div class="main-header container mt-3">
    <div class="row mx-0">

      <div class="col-12 what-we-do-div mb-3">
        <h2>GET IN TOUCH WITH US</h2>
      </div>

      <div class="col-12 mb-3 text-start">
        <form class="row mx-0">
          <div class="form-group col-md-6 mb-5">
            <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp"
                   placeholder="Name *">
          </div>
          <div class="form-group col-md-6 mb-5">
            <input type="text" class="form-control" id="exampleInputEmail2" aria-describedby="emailHelp"
                   placeholder="Company *">
          </div>
          <div class="form-group col-md-6 mb-5">
            <input type="text" class="form-control" id="exampleInputEmail3" aria-describedby="emailHelp"
                   placeholder="Phone *">
          </div>
          <div class="form-group col-md-6 mb-5">
            <input type="text" class="form-control" id="exampleInputEmail4" aria-describedby="emailHelp"
                   placeholder="Email *">
          </div>

          <div class="form-group col-md-12 mt-5">
            <textarea rows="1" type="text" class="form-control" id="exampleInputEmail5" aria-describedby="emailHelp"
                      placeholder="Message *"></textarea>
          </div>
        </form>
      </div>
      <div class="col-12 right">
        <button class="btn know-btn">Submit</button>
      </div>

      <div class="col-md-7 text-center contact-text mx-auto">
        You can also mail us to hello@phosphenes.co & we shall get back to you at the earliest.

        <span class="mt-4 mb-3 d-block">Address: PO Box 692761, Dubai, UAE</span>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'ContactUs',
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

.contact-text {
  font-size: 24px;
  font-family: SourceRegular;
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

form {
  background-color: #f2f2f2;
  padding: 20px;

  input, textarea {
    font-family: SourceRegular;
    font-size: 24px;
    color: #333333 !important;
    border: none !important;
    border-radius: 0;
    padding-left: 0 !important;
    border-bottom: 2px solid #333333 !important;
    background-color: transparent;

    &::placeholder {
      color: #333333 !important;
    }

    &:focus {
      outline: none !important;
      border: none !important;
      box-shadow: none !important;
      color: #333333 !important;
      border: none !important;
      border-radius: 0;
      padding-left: 0 !important;
      border-bottom: 2px solid #333333 !important;
      background-color: transparent;
    }
  }
}
</style>
