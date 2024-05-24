<script>
    export default {
        name: "AppHeader",
        // data() {
        //     return {
        //         links: [
        //         "CHARACTERS",
        //             "MOVIES",
        //             "TV",
        //             "GAMES",
        //             "COLLECTIBLES",
        //             "VIDEOS",
        //             "FANS",
        //             "NEWS",
        //             "SHOP"
        //         ]
        //     }
        // } 
    }
</script>

<template>
    <header>
        <!-- Contenitore -->
        <div class="container">
            <div>
                <!-- <img class="logo" src="../assets/img/dc-logo.png" alt=""> -->
            </div>
            <div class="linkContainer">
                <!-- <ul>
                    <li class="link" v-for="link in links" :key="link">
                        {{link}}
                    </li>
                </ul> -->
            </div>
        </div>
    </header>
</template>

<style>
    header {
        background-color: orange;
        width: 100%;
        height: 10rem;
    }
</style>