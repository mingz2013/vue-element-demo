<template>
    <div>
        <img alt="Vue logo" src="../assets/logo.png">
        <HelloWorld msg="Welcome to Your Vue.js App"/>

        <div id="nav">
            <router-link to="/">Home</router-link>
            |
            <router-link to="/about">About</router-link>
        </div>

        <router-view/>

        <img src="../assets/logo.png">
        <div>
            <p>
                If Element is successfully added to this project, you'll see an
                <code v-text="'<el-button>'"></code>
                below
            </p>
            <el-button>el-button</el-button>
        </div>
        <HelloWorld msg="Welcome to Your Vue.js App"/>
    </div>

</template>

<script>
    import HelloWorld from './HelloWorld.vue'

    export default {
        name: 'demo',
        components: {
            HelloWorld
        }
    }
</script>