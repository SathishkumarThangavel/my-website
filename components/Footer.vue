<template>
    <div class="footer">
        <div class="contact">
            <a href="https://twitter.com/ITsathishkumar" target="_blank" rel="noopener noreferrer" title="twitter">
                <twitterLogo />
            </a>
            <a href="https://github.com/SathishkumarThangavel" target="_blank" rel="noopener noreferrer" title="github">
                <githubLogo />
            </a>
            <a href="https://www.linkedin.com/in/sathishkumarthangavel/" target="_blank" rel="noopener noreferrer" title="linkedin">
                <linkedinLogo />
            </a>
        </div>
        <div class="powered"> © Sathishkumar Thangavel. Powered by <a href="https://nuxtjs.org/" target="_blank" rel="noopener noreferrer">Nuxtjs</a></div>
    </div>
</template>
<script>
import twitterLogo from "~/assets/twitter.svg?inline";
import githubLogo from "~/assets/github.svg?inline";
import linkedinLogo from "~/assets/linkedin.svg?inline";

export default {
    name: 'footer',
    components: { twitterLogo, githubLogo, linkedinLogo },
}
</script>
<style>
.footer {
    margin-top: 40px;
    max-width: 50%;
    margin: 50px auto;
}
.footer svg {
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