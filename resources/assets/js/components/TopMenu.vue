<template>
    <nav class="navbar navbar-toggleable-md navbar-light bg-faded">
        <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <a class="navbar-brand" href="#">Navbar</a>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto">
                <li class="nav-item">
                    <router-link class="nav-link" to="/">Index</router-link>
                </li>
                <li class="nav-item">
                    <router-link class="nav-link" :to="'/users'">Users</router-link>
                </li>
            </ul>
        </div>
    </nav>
</template>
<script>
    export default {
        mounted() {
            console.log('Component Top menu mounted.')
        },
        data() {
            return {
                username: 'username template'
            }
        }
    }
</script>
<style>
    .navbar {
        margin-bottom: 20px;
    }
</style>