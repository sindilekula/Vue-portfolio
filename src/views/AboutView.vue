<template>
<section id="about">
  <div class="about">
    <h1>Know Me More</h1>

    <div class="row">
      <div class="col-lg-3">
        <div class="personal-image mt-5">
          <p class="text-light"><span class="fw-bold">Name:</span><span class="ms-3">Sindile Kula</span></p>
          <p class="text-light"><span class="fw-bold">Email:</span><span class="ms-3">Kulasindile@gmail.com</span></p>
          <img src="../assets/koko2.png" alt="" class="img-fluid">
        </div>
      </div>
      <div class="col-lg-6">
        <div class="bio mt-5">
        <h3 class="text-white">I am <span class="name">Sindile Kula,</span> a aspiring web developer.</h3>
        <p class="text-muted">I'm a young man ready to learn new things. I can simply adjust to any situation. I work hard while also being intelligent. I'm great at multitasking and keeping track of time. Prior to any endeavor, I appreciate planning.</p>
        <p class="text-muted">I'm a really creative person who is also very committed to my profession. I enjoy new challenges since they force me to improve in all areas. I also consider myself to be someone who performs well under duress.</p>
        <p class="text-muted">I'm a great team player, have excellent communication abilities, and am an excellent listener, to name a few. I'm really adaptable, and I always deliver the end results.</p>
        </div>

        <div class="details">
          <p class="text-light"><span class="fw-bold">Name:</span><span class="ms-3">Sindile Kula</span></p>
          <p class="text-light"><span class="fw-bold">Email:</span><span class="ms-3">Kulasindile@gmail.com</span></p>
          <p class="text-light"><span class="fw-bold">Age:</span><span class="ms-3">23</span></p>
          <p class="text-light"><span class="fw-bold">From:</span><span class="ms-3">Cape Town, Gugulethu</span></p>
        </div>

        <div class="button">
          <a href="/CV_2021-12-16-034328.pdf" download="">
            <button type="button" class="btn btn-lg rounded-pill mt-3">Download CV</button>
          </a>
        </div>
      </div>
      <div class="col-lg-3">
        <div class="personal-image mt-5">
          <p class="text-light"><span class="fw-bold">Age:</span><span class="ms-3">23</span></p>
          <p class="text-light"><span class="fw-bold">From:</span><span class="ms-3">Cape Town, Gugulethu</span></p>
          <img src="../assets/koko.png" alt="" class="img-fluid">
        </div>
      </div>
    </div>
  </div>
</section>
</template>

<script>
export default {
  
}
</script>
<style scoped>
  #about {
    background-image: linear-gradient(to bottom, #000000, #151313, #231f1f, #312b2a, #3f3835, #544238, #694c39, #7c5739, #9b6030, #bb6726, #dc6d18, #ff7200);
    min-height: 100vh;
    width: 100%;
  }

  .about h1 {
    font-weight: 600;
    color: white;
    /* text-decoration: underline; */
    text-shadow: 1px 1px 1px black;
    position: relative;
    cursor: pointer;
  }

  .about h1:before {
    content: '';
    width: 10%;
    height: 1px;
    position: absolute;
    left: 45%;
    bottom: -8px;
    border-bottom: solid 4px #ff7200;
  }

  .details {
    display: none;
  }

  .bio {
    font-size: 20px;
  }

  button.btn {
    background-color: #ff7200;
    color: #000000;
  }

  button.btn:hover {
    background-color: #000000;
    color: white;
  }

  @media screen and (max-width: 992px) {
    .personal-image {
      display: none;
    }

    .details {
      display: block;
    }

  }
</style>
