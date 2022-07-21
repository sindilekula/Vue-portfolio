<template>
    <section id="footer" class="text-center">
        <div class="container text-center">
             <div class="social-media">
                <a target="_blank" href="https://github.com/sindilekula"><i class="fa-brands fa-github text-light" data-toggle="tooltip" data-placement="top" title="Github"></i></a>
                <a target="_blank" href="https://www.linkedin.com/in/sindile-kula-2b777a238/"><i class="fa-brands fa-linkedin text-light ms-5" data-toggle="tooltip" data-placement="top" title="Linkedin"></i></a>
                <a target="_blank" href="https://codepen.io/sindilekula"><i class="fa-brands fa-codepen text-light ms-5" data-toggle="tooltip" data-placement="top" title="Codepen"></i></a>
                <a target="_blank" href="https://accounts.google.com/"><i class="fa-brands fa-google text-light ms-5" data-toggle="tooltip" data-placement="top" title="Google"></i></a>
            </div>
            <div class="footer-names mt-5">
                <ul class="list">
                    <li>Sitemap</li>
                    <li>About</li>
                    <li>Need Help?</li>
                    <li>Content Guide</li>
                    <li>Privacy</li>
                    <li>Terms of use</li>
                    <li>Advertising</li>
                </ul>
            </div>
            <div class="copyright">
                <p class="">Copyright © 2022 <span class="name">Sindile</span>. All rights reserved.</p>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    #footer {
        background-color: black;
        height: 220px;
    }

    .social-media a .fa-brands {
        border: solid 1px #ff7200;
        height: 30px;
        width: 30px;
        border-radius: 20px;
    }

    ul {
        display: flex;
        justify-content: space-between;
        list-style-type: none;
    }

    .name {
        color: #ff7200;
    }

    a.fa-brands:hover {
        color: #ff7200;
    }

    @media screen and (max-width: 768px) {
        ul.list li {
            font-size: 10px;
        }
    }
</style>