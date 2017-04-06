<template>
    <header>
        <Menu mode="horizontal" theme="dark" active-name="1">
            <div class="layout-logo"></div>
            <div class="layout-nav">
                <Menu-item name="1">
                    <Icon type="ios-navigate"></Icon>
                    <router-link to="/">首页</router-link>
                </Menu-item>
                <Menu-item name="2">
                    <Icon type="ios-keypad"></Icon>
                    <router-link to="/detail">子模块</router-link>
                </Menu-item>
            </div>
        </Menu>
    </header>
</template>
<script type="text/javascript">
export default{
    data() {
        return{
             title:'直播屋'
        }
    }
}
</script>
<style>

</style>