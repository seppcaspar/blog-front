<template>
    <b-navbar>
        <template #brand>
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                <img
                    src="https://raw.githubusercontent.com/buefy/buefy/dev/static/img/buefy-logo.png"
                    alt="Lightweight UI components for Vue.js based on Bulma"
                >
            </b-navbar-item>
        </template>
        <template #start>
            <b-navbar-item tag="router-link" to="/">
                Home
            </b-navbar-item>
            <b-navbar-item tag="router-link" to="/todo">
                Todo
            </b-navbar-item>
        </template>

        <template #end>
            <b-navbar-item tag="div">
                <div class="buttons">
                    <RouterLink to="/Register" class="button is-primary">
                        Sign up
                    </RouterLink>
                    <RouterLink to="/login" class="button is-light">
                        Log in
                    </RouterLink>
                </div>
            </b-navbar-item>
        </template>
    </b-navbar>
</template>