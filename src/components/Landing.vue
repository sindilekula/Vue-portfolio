<template>
<div class="container">
  <div class="hello">
    <div class="row">
      <div class="col-lg-8">
        <div class="intro-msg">
          <h1>Hi, I'm <span class="name">Sindile Kula</span></h1>
          <p>An <span class="aspire">Aspiring</span> Web Developer!</p>
          <a href="#contact">
            <button type="button" class="btn btn-lg rounded-pill mt-5">Hire Me</button>
          </a>
        </div>
      </div>
      <div class="col-lg-4 mt-1">
        <div class="personal-image">
          <img src="../assets/sindi.png" alt="" class="img-fluid">
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
    background-image: linear-gradient(to bottom, #000000, #151313, #231f1f, #312b2a, #3f3835, #544238, #694c39, #7c5739, #9b6030, #bb6726, #dc6d18, #ff7200);
    }

    .img-fluid {
      height: 600px;
      position: relative;
      animation: up-down 1.9s infinite ease-in-out alternate;
    }

    @keyframes up-down{
    from{
    transform: translatey(10px);
  }
    to{
    transform: translatey(-10px);
  }
}

    .col-lg-4 {
      margin-top: 200px;
    }

     .col-lg-8 {
      display: flex;
      justify-content: flex-start;
      margin-top: 200px;
    }

    .intro-msg {
      margin-left: 20px;
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
