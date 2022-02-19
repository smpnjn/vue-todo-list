<template>
    <div id="nav">
        <router-link to="/">Home</router-link> |
        <router-link to="/archive">Archive</router-link> |
        <router-link to="/about">About</router-link>
    </div>
    <router-view/>
</template>

<script>
import { useStore } from 'vuex'
export default {
	beforeCreate() {
        const store = useStore()
		store.commit('loadStore');
	}
}
</script>

<style>
#app {
  font-family: Inter, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#nav a {
    font-weight: bold;
    color: #2c3e50;
}

#nav a.router-link-exact-active {
    color: #42b983;
}
</style>
