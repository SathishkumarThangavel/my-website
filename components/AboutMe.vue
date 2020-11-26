<template>
    <div class="section-container"> 
        <div class="introduction"></div>
        <h2>Tech I know</h2>
        <ul>
            <li><img src="~/assets/vuejs.svg"> Vuejs, <img src="~/assets/preactjs.svg"> PreactJs, <img src="~/assets/emberjs.svg"> Emberjs, <img src="~/assets/stenciljs.png"> Stenciljs</li>
            <li> SCSS/CSS, LESS/CSS, Bootstrap, ElementUI</li>
            <li>Hugo Js, NuxtJs, Gatsby/GraphQL</li>
            <li>Git, Gulp, npm/yarn</li>
            <li><b>Tools:</b> VScode/Atom code editor, Adobe XD/Figma</li>
        </ul>

        <div id="personal-projects">
            <h2 >Personal Projects</h2>
            <section v-on:click="openWindow('https://web-components-kappa.vercel.app/')">
                <img src="~/assets/toast.svg">
                <div>
                    <h3>Toast Web Component</h3>
                    <p>Easy-to-use toast component built on stenciljs with web components concept.</p>
                </div>
            </section>
            <section v-on:click="openWindow('https://www.npmjs.com/package/ember-simple-range-slider')">
                <img src="~/assets/slider.svg">
                <div>
                    <h3>Ember Range Slider</h3>
                    <p>A node module can be used in emberjs as addon. Range slider with consistent design across browser</p>
                </div>
            </section>
        </div>

        <h2 id="work-experience">Work Experience</h2>
        <!-- Freshworks -->
        <div class="experience">
            <div class="company">
                <img src="~/assets/freshworks.svg" class="logo" alt="">
                <h3>Freshworks</h3>
                <a target="_blank" href="https://www.freshworks.com" rel="noopener noreferrer">
                    <img src="~/assets/openlink.svg" class="open-external-link" alt="">
                </a>
            </div>
            <div class="period">
                Chennai, India - (Oct 2019 - Present)
            </div>
            <div class="project">
                <h3>Tech team - Platform</h3>
                <p>Enhance the developer platform, Requirement analysis, design, develop, review codes, support developer community and organization maintained open source contribution</p>
            </div>
        </div>
        <hr>
        <!-- Zoho -->
        <div class="experience">
            <div class="company">
                <img src="~/assets/zoho.png" class="logo" style="width:100px;height:auto" alt="Zoho">
                <h3>Corporation Pvt. Ltd</h3>
                <a target="_blank" href="https://www.zoho.com" rel="noopener noreferrer">
                    <img src="~/assets/openlink.svg" class="open-external-link" alt="">
                </a>
            </div>
            <div class="period">
                Chennai, India - (May 2016 - Oct 2019)
            </div>
            <div class="project">
                <h3>UI Team - Product</h3>
                <p> Enhance Product Features, add unit and integration tests, peer code reviews, requirement gathering, Mentor new team member  </p>
                <h3>UI Team - Marketing</h3>
                <p> Build Customer experiencing marketing websites, enhance performance, improve SEO, make website responsive and smooth transitions </p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'about-me',
    methods: {
        openWindow(link) {
            window.open(link, '_blank');
        }
    }
}
</script>
<style scoped>
    .section-container {
        max-width: 50%;
        margin: 50px auto;
    }
    h2 {
        margin: 35px 0 20px;
    }
    #personal-projects section {
        padding: 20px;
        background-color: #d1f9f9;
        cursor: pointer;
        display: flex;
        align-items: center;
        line-height: 1.6em;
        margin: 20px 0;
    }
    #personal-projects h3 {
        font-size: 16px;
        color: #0e04b1;
    }
    #personal-projects section img {
        width: 30px;
        height: 30px;
        margin-right: 25px
    }
    li {
        padding: 5px 0;
    }
    li img {
        width: 15px;
        height: 15px;
        margin: 0;
    }
    .experience {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
    }
    .company {
        display: flex;
        -webkit-box-align: center;
        align-items: center;
        margin-top: 0.5rem;
        margin-bottom: 0.5rem;
    }
    .logo {
        width: 40px;
        height: 40px;
        margin-right: 0.5rem;
    }
    h3 {
        font-size: 24px;
    }
    .open-external-link {
        width: 12px;
        height: 12px;
        margin-left: 15px;
        opacity: 0.3;
    }
    .open-external-link:hover {
        opacity: 1;
    }
    .period {
        font-family: Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
        margin-bottom: 0.5rem;
        color:#6d6b6b;
    }
    .project h3 {
        font-size: 18px
    }
    .project p {
        font-family: Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
        margin-top: 5px;
        margin-bottom: 10px;
        line-height: 1.5em;
    }
    hr {
        border-width: 0px 0px 0.0625rem;
        opacity: 0.6;
        margin-top: 0.5rem;
        margin-bottom: 0.5rem;
        border-color: rgb(74, 85, 104);
    }
    @media screen and (max-width: 600px) {
        .section-container {
            max-width: 80%;
        }
    }
</style>