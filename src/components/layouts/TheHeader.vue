<template>
    <div class="navbar navbar-default topnav">
        <div class="container">
            <div class="navbar-header">
                <a href="/" class="navbar-brand">
                    <img :src="logo.src" :alt="logo.title">
                    <span class="title">{{ logo.title }}</span>
                </a>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'TheHeader',
        data() {
            return {
                logo: {
                    src: `${this.uploadsUrl}communities/hIZjRRdF8oVYZy69XJnT.png!/both/44x44`,
                    title: 'Learnku Vue.js'
                }
            }
        },
        beforeCreate() {
            this.uploadsUrl = 'https://cdn.learnku.com//uploads/'
        }
    }
</script>

<style scoped>
    .title { color: black;}
    .navbar-brand > img { display: inline-block; }
    .navbar-default .navbar-nav > .active > a { background: rgba(0,0,0,.03);}
</style>
