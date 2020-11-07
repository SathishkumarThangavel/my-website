<template>
    <div class="footer">
        <div class="contact">
        <a href="https://twitter.com/ITsathishkumar">
            <img src="~/assets/twitter.svg" alt="twitter">
        </a>
        <a href="https://github.com/SathishkumarThangavel">
            <img src="~/assets/github.svg" alt="github">
        </a>
        <a href="https://www.linkedin.com/in/sathishkumarthangavel/">
            <img src="~/assets/linkedin.svg" alt="linkedin">
        </a>
        </div>
        <div class="powered"> © Sathishkumar Thangavel. Powered by <a href="https://nuxtjs.org/">Nuxtjs</a></div>
    </div>
</template>
<script>
export default {
    name: 'footer',
}
</script>
<style>
.footer {
    margin-top: 40px;
    max-width: 50%;
    margin: 50px auto;
}
img {
    width: 20px;
    height: 20px;
    margin-right: 10px;
}
.contact {
    text-align: center;
}
.powered {
    margin-top: 10px;
    text-align: center
}
</style>