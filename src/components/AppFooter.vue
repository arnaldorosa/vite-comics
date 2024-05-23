<script>
    export default {
        name: "AppFooter"
    }
</script>

<template>
    <footer>
        <section class="s1">
            <div></div>
        </section>
        <section class="s2">
            <div></div>
            <div></div>
        </section>
        <section class="s3">
            <div></div>
            <div></div>
        </section>
    </footer>
</template>

<style>
    .s1 {
        background-color: darkgoldenrod;
        width: 100%;
        height: 10rem;
    }

    .s2 {
        background-image: url(/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        width: 100%;
        height: 27.2rem;
    }

    .s3 {
        background-color: darkslateblue;
        width: 100%;
        height: 10rem;
    }
</style>