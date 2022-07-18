<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-dark">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">Sindile.K</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                <li class="nav-item">
                <a class="nav-link active text-light ms-5" aria-current="page" href="#">Home</a>
                </li>
                <li class="nav-item">
                <a class="nav-link text-light ms-5" href="#">About Me</a>
                </li>
                <li class="nav-item">
                <a class="nav-link text-light ms-5" href="#">Resume</a>
                </li>
                <li class="nav-item">
                <a class="nav-link text-light ms-5" href="#">Portfolio</a>
                </li>
                <li class="nav-item">
                <a class="nav-link text-light ms-5" href="#">Contact</a>
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
    color: #ff7200;
}

</style>