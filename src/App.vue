<template>
    <div id="app">
        <!--<firstcomponent></firstcomponent>-->
        <YoHeader></YoHeader>
        <div class="layout-content">
            <router-view></router-view>
        </div>
        <YoFooter></YoFooter>
    </div>
</template>

<script>
    //导入组件
    import YoHeader from './layout/Header.vue'
    import YoFooter from './layout/Footer.vue'
    export default {
        name: 'app',
//        components:{Header,Footer},
        data () {
            return {
                msg: 'Welcome to Your Vue.js App'
            }
        },
        components: { YoHeader,YoFooter}
    }
</script>

<style>
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;

    }

    h1, h2 {
        font-weight: normal;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }
    body{
        background: #eee!important;
    }

</style>
