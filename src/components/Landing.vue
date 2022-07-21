<template>
<div class="container">
  <div class="hello">
    <!-- <h1>{{ msg }}</h1> -->
    <div class="row">
      <div class="col-lg-8">
        <div class="intro-msg ms-5">
          <h1>Hi, I'm <span class="name">Sindile Kula</span></h1>
          <p>An <span class="aspire">Aspiring</span> Web Developer!</p>
          <a href="#contact">
            <button type="button" class="btn btn-lg rounded-pill mt-5">Hire Me</button>
          </a>
        </div>
      </div>
      <div class="col-lg-4 mt-1">
        <div class="personal-image">
          <img src="../assets/sindi.png" alt="" class="img-fluid"> -->
        </div>
      </div>
    </div>
  </div>

</div>
</template>

<script>
export default {
  name: 'Landing',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

 * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        scroll-behavior: smooth;
    }

    .hello {
        width: 100vw;
        min-height: 100vh;
        overflow: hidden;
        /* background: linear-gradient(to top, rgba(0,0,0,0.5)50%, rgba(0,0,0,0.5)50%,), url("https://cdn.pixabay.com/photo/2016/11/29/08/15/beach-1868342_960_720.jpg"); */
        /* background-image: url("https://cdn.pixabay.com/photo/2017/11/24/21/49/bali-2975787_960_720.jpg");
        background-position: center;
        background-size: cover; */
        /* https://cdn.pixabay.com/photo/2017/11/24/21/49/bali-2975787_960_720.jpg
        https://cdn.pixabay.com/photo/2016/11/29/08/15/beach-1868342_960_720.jpg */
        /* background: linear-gradient(
      0deg,
      rgba(65, 67, 69, 0.6589986336331408) 0%,
      rgba(35, 37, 38, 0.8802871490393032) 100%
    ),
    url(./assets/cape-town.jpg) no-repeat top center; */
    background-image: linear-gradient(to bottom, #000000, #151313, #231f1f, #312b2a, #3f3835, #544238, #694c39, #7c5739, #9b6030, #bb6726, #dc6d18, #ff7200);
    /* background-size: cover;
    background-position: center; */
    }

    .img-fluid {
      height: 600px;
      position: relative;
    }

    .col-lg-4 {
      margin-top: 200px;
    }

     .col-lg-8 {
      display: flex;
      justify-content: flex-start;
      margin-top: 200px;
    }

    .intro-msg h1{
      font-size: 80px;
      text-shadow: 1px 1px 1px white;
    }

    .intro-msg p{
      font-size: 30px;
      text-shadow: 1px 1px 1px white;
    }

    .name {
       color: #ff7200;
       font-size: 120px;
    }

    .aspire {
       color: #ff7200;
       font-size: 60px;
       text-decoration: underline;
    }

    button.btn {
      width: 200px;
      background-color: #ff7200;
      border: solid 1px black;
    }

    button.btn:hover {
      width: 200px;
      color: white;
      background-color: black;
      border: solid 1px #ff7200;
    }

    @media screen and (max-width: 584px) {
      .intro-msg h1 {
        font-size: 30px;
      }

      .hello {
        overflow: hidden;
      }
    }
</style>
