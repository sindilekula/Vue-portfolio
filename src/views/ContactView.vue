<template>
<section id="contact">
  <div class="container">
    <h1 class="heading">Get In Touch</h1>
    <ul class="details">
        <li><p><span class="icon ms-2"><i class="fa-solid fa-phone ms-2"></i></span>:084 384 2221</p></li>
        <li><p><span class="icon"><i class="fa-solid fa-envelope ms-2"></i></span>:Kulasindile@gmail.com</p></li>
        <li><p><span class="icon"><i class="fa-solid fa-location-dot ms-2"></i></span>:206 Ny21, Gugulethu, 7750</p></li>
    </ul>
    <form target="_blank" action="https://formspree.io/f/xqknwllo" method="post">
        <div class="row mt-5">
            <div class="col-lg-6">
                <input type="text" name="name" class="name my-3 text-white" placeholder="Enter your name..." required>
                <input type="email" name="email" class="email my-3 text-white" placeholder="Enter your email..." required>
                <input type="text" name="phone" class="phone my-3 text-white" placeholder="Enter your phone number..." required>
            </div>
            <div class="col-lg-6">
                <textarea id="message" class="message my-3 text-white" placeholder="Type your message..."></textarea>
            </div>
            <div class="button mb-3">
                <button type="submit" class="btn btn-lg rounded-pill">Send message</button>
            </div>
        </div>
    </form>
    <!-- <div class="row d-flex flex-column">
    <div class="following">
        <p>Follow Me</p>
        <div class="social-media">
        <a target="_blank" href="https://github.com/sindilekula"><i class="fa-brands fa-github text-light" data-toggle="tooltip" data-placement="top" title="Github"></i></a>
        <a target="_blank" href="https://www.linkedin.com/in/sindile-kula-2b777a238/"><i class="fa-brands fa-linkedin text-light ms-3" data-toggle="tooltip" data-placement="top" title="Linkedin"></i></a>
        <a target="_blank" href="https://codepen.io/sindilekula"><i class="fa-brands fa-codepen text-light ms-3" data-toggle="tooltip" data-placement="top" title="Codepen"></i></a>
        <a target="_blank" href="https://accounts.google.com/"><i class="fa-brands fa-google text-light ms-3" data-toggle="tooltip" data-placement="top" title="Google"></i></a>
        </div>
                        
    </div>
    </div> -->
  </div>
</section>
</template>
<script>
export default {};
</script>
<style scoped>
#contact {
  background: 
    /* top, transparent red, faked with gradient */ linear-gradient(
      rgb(211, 95, 0),
      rgba(0, 0, 0, 0.985)
    ),
    /* bottom, image */ url(@/assets/earth.jpg);

  background-size: cover;
  background-position: center;
  background-blend-mode: overlay;
  width: 100%;
  min-height: 100vh;
  background-color: rgba(0, 0, 0, 0.2);
}

.heading {
    font-weight: 600;
    color: white;
     /* text-decoration: underline; */
    text-shadow: 1px 1px 1px black;
    position: relative;
    cursor: pointer;
}

.heading:before {
    content: '';
    width: 10%;
    height: 1px;
    position: absolute;
    left: 45%;
    bottom: -8px;
    border-bottom: solid 4px #ff7200;
}

.details {
    color: white;
     text-shadow: 1px 1px 1px black;
    list-style-type: none;
    margin-top: 80px;
    /* background-color: rgba(0, 0, 0, 0.2); */
    /* height: 150px;
    width: 400px; */
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-size: 25px;
}

.icon {
    color: #ff7200;
}

.col-lg-6 {
    display: flex;
    flex-direction: column;
    margin-top: 50px;
}

input {
    height: 40px;
    background-color: rgba(0, 0, 0, 0.2);
    border: solid 1px #ff7200;
}

.message {
    height: 190px;
    background-color: rgba(0, 0, 0, 0.2);
    border: solid 1px #ff7200;
}

.btn {
    background-color: #ff7200;
    color: black;
}

.btn:hover {
    background-color: black;
    color: white;
}

.following {
    display: flex;
    justify-content: flex-start;
}

.following p {
    color: white;
    font-size: 20px;
}

.social-media {
    display: flex;
}

@media screen and (max-width: 584px) {
    #contact {
        overflow: hidden;
    }

    .col-lg-6 {
        width: 600px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    input {
        width: 300px;
    }

    #message {
        width: 300px;
    }
}

</style>
