<template >
    <div id="centerCallToAction">
        <div>
            <h1>
                <b>Wayfinder - depression</b>
            </h1>
            <p>Login or Register</p>
        </div>
    </div>
    <div></div>
    <div>
        <router-link to="login">
            Login
        </router-link>
        <router-link to="register">
            Register
        </router-link>
    </div>
</template>

<script setup></script>

<style lang="scss">
    #centerCallToAction {
        color: red;
    }
</style>