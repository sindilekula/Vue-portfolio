<template>
    <section id="testimonials">
        <div class="testimonials">
            <h1>What People Say<span class="emphasis ms-2"><i class="fa-solid fa-exclamation"></i></span></h1>
            <div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
                <div class="carousel-inner">
                    <div v-for="(testimonial, index) in testimonials" :key="index" :class="{ active: index === 0}" class="carousel-item">
                        <div class="card p-5 mt-5">
                                <div class="details">
                                    <img :src="testimonial.imgURL" class="img-fluid rounded-circle" alt="..." style="width: 150px; height: 150px; object-fit: cover;">
                                    <div class="info d-flex flex-column ms-3">
                                        <p class="name">{{ testimonial.name }}</p>
                                        <p class="text-muted">{{ testimonial.relationship }}</p>
                                    </div>
                                </div>
                                <div class="reviews">
                                    <p class="text-white mt-5">"{{ testimonial.message }}"</p>
                                </div>
                                <div class="ratings mt-3">
                                    <i class="fa-solid fa-star"></i>
                                    <i class="fa-solid fa-star"></i>
                                    <i class="fa-solid fa-star"></i>
                                    <i class="fa-solid fa-star"></i>
                                    <i class="fa-solid fa-star"></i>
                                </div>
                        </div>
                    </div>
                </div>
                <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                </button>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    data() {
        return {
            testimonials: [
                {
                    imgURL: "https://i.postimg.cc/7P5JV5XM/Lihle-1.jpg",
                    name: "Lihle Goliath",
                    relationship: "From Life Choices Academy",
                    message: "Kula Sindile, an individual who is dedicated and motivated to attain his objectives at whatever costs. He is dependable and works well with others.",
                },
                {
                    imgURL: "https://i.postimg.cc/kgny7L0g/Leandre-5.jpg",
                    name: "Le-Andre Moritz",
                    relationship: "From Life Choices Academy",
                    message: "Sindile is the sort of person that is always striving to better and be the greatest version of himself. In the workplace, his gentle and open-minded personality makes him a pleasure to be around.",
                },
                {
                    imgURL: "https://i.postimg.cc/kG6pFLJm/Raaid-3.jpg",
                    name: "Raaid Abdullatief",
                    relationship: "From Life Choices Academy",
                    message: "Sindile Kula, His dedication to his profession is absolutely extraordinary. He is a pleasure to deal with and constantly prioritizes his clients.",
                },
                {
                    imgURL: "https://i.postimg.cc/d1mxWGdW/Siyolise-4.jpg",
                    name: "Siyolise Mekuto",
                    relationship: "From Life Choices Academy",
                    message: "Sindile Kula is a determined individual. He goes above and above to assist people and is a pleasure to be around.",
                },
                {
                    imgURL: "https://i.postimg.cc/k4rDphmP/Live-1.jpg",
                    name: "Live Maweni",
                    relationship: "From Life Choices Academy",
                    message: "Sindile is an immensely resilient person who is also incredibly creative, intelligent, and hardworking. He's not simply a pleasure to work with; in fact, it's astounding to see just how much time and attention he puts into each project.",
                },
                {
                    imgURL: "https://i.postimg.cc/FRLDq3St/jason.jpg",
                    name: "Jason Wandrag",
                    relationship: "From Life Choices Academy",
                    message: "Sindile is a hardworking and motivated student who has put in a lot of effort in his studies. His work and approach have steadily improved. I wish him well in his future endeavors.",
                },
            ]
        }
    }
}
</script>
<style scoped>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

#testimonials {
    background-image: linear-gradient(to bottom, #000000, #151313, #231f1f, #312b2a, #3f3835, #544238, #694c39, #7c5739, #9b6030, #bb6726, #dc6d18, #ff7200);
    min-height: 100vh;
    width: 100%;
}

.testimonials h1 {
    font-weight: 600;
    color: white;
    text-shadow: 1px 1px 1px black;
    position: relative;
    cursor: pointer;
}
.testimonials h1:before {
    content: '';
    width: 10%;
    height: 1px;
    position: absolute;
    left: 45%;
    bottom: -8px;
    border-bottom: solid 4px #ff7200;
}

.emphasis {
    color: #ff7200;
}

.ratings {
    color: #ff7200;
}

.carousel-item {
     transition: transform 3s ease-in-out;
}

.details {
    display: flex;
    flex-direction: row;
}

.card {
    background-color: rgba(0, 0, 0, 0.2);
    width: 600px;
    height: fit-content;
    box-shadow: 2px 2px 3px 2px #000000;
    font-size: 20px;
    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 50%;  
}

.img-fluid {
    object-fit: cover;
}

p.name {
    color: #ff7200;
    text-shadow: 1px 1px 1px black;
    position: relative;
    cursor: pointer;

}

@media screen and (max-width: 520px) {
    .details {
        display: flex;
        flex-direction: column;
    }
}

</style>