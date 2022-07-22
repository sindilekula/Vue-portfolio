<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-dark">
        <div class="container-fluid">
            <a class="navbar-brand" href="#"><span class="first-letter">S</span>indile.</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation" onclick="toggleNav()">
            <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                <li class="nav-item">
                <router-link class="nav-link active text-light ms-5" aria-current="page" href="#" to="/">Home</router-link>
                </li>
                <li class="nav-item">
                <router-link class="nav-link text-light ms-5" href="#" to="/about">About</router-link>
                </li>
                <li class="nav-item">
                <router-link class="nav-link text-light ms-5" href="#" to="/resume">Resume</router-link>
                </li>
                <li class="nav-item">
                <router-link class="nav-link text-light ms-5" href="#" to="/projects">Projects</router-link>
                </li>
                <li class="nav-item">
                <router-link class="nav-link text-light ms-5" href="#" to="/testimonials">Testimonials</router-link>
                </li>
                <li class="nav-item">
                <router-link class="nav-link text-light ms-5" href="#" to="/contact">Contact</router-link>
                </li>
            </ul>
            <!-- <form class="d-flex">
                <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                <button class="btn btn-outline-success" type="submit">Search</button>
            </form> -->
            </div>
        </div>
    </nav>
</template>
<script>
export default {
    
}
</script>
<style>
#navbarSupportedContent {
    margin-left: 200px;
}

.container-fluid {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
}

.navbar {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    font-family: Cormorant SC;
    font-size: 20px;
    background-color: black;
    width: 100%;
}

.navbar-light .navbar-brand {
    /* margin-left: 100px; */
    color: white;
    font-size: 20px;
}

.first-letter {
    color: #ff7200;
    font-size: 40px;
}

nav ul li a {
    position: relative;
}

nav ul li a::after {
    content: '';
    width: 0;
    height: 3px;
    background: #ff7200;
    position: absolute;
    left: 0;
    bottom: -6px;
    transition: 0.5s;
}

nav ul li a:hover::after{
    width: 100%;
}

vbar>.container, .navbar>.container-fluid, .navbar>.container-lg, .navbar>.container-md, .navbar>.container-sm, .navbar>.container-xl, .navbar>.container-xxl {
    justify-content: center;
}

ul li.nav-link {
    margin-left: 100px;
}

.collapse {
    display: flex;
    justify-content: center;
}

</style>