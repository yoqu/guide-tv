<template>
    <header>
        <Menu mode="horizontal" theme="light" active-name="1" @on-select="menuJump">
            <div class="layout-logo"></div>
            <div class="layout-nav">
                <Menu-item name="/">
                        <Icon type="ios-navigate"></Icon>
                        所有直播
                </Menu-item>
                <Menu-item name="/detail">
                        <Icon type="ios-keypad"></Icon>
                        休闲娱乐
                </Menu-item>
                <Menu-item name="/detail">
                    <Icon type="ios-keypad"></Icon>
                    世界杯
                </Menu-item>
            </div>
        </Menu>
        <Menu mode="horizontal" active-name="1">
            <div class="layout-assistant">
                <Menu-item name="1">斗鱼</Menu-item>
                <Menu-item name="2">熊猫</Menu-item>
                <Menu-item name="3">龙珠</Menu-item>
                <Menu-item name="4">全民</Menu-item>
            </div>
        </Menu>
    </header>
</template>
<script type="text/javascript">
    export default{
        data() {
            return {
                title: '直播屋'
            }
        },
        methods: {
            menuJump (data){
                this.$router.push(data);
            }
        }
    }
</script>
<style>
    .layout {
        border: 1px solid #d7dde4;
        background: #f5f7f9;
    }

    .layout-logo {
        width: 100px;
        height: 30px;
        background: #5b6270;
        border-radius: 3px;
        float: left;
        position: relative;
        top: 15px;
        left: 20px;
    }

    .layout-nav {
        width: 420px;
        margin: 0 auto;
    }

    .ivu-menu-light .layout-nav .ivu-menu-item a {
        color: #657180;
    }

    .ivu-menu-light .layout-nav .ivu-menu-item-active a {
        color: #39f;

    }

    .layout-assistant {
        width: 300px;
        margin: 0 auto;
        height: inherit;
    }

    .layout-breadcrumb {
        padding: 10px 15px 0;
    }

    .layout-content {
        min-height: 200px;
        margin: 15px;
        overflow: hidden;
    }

    .layout-content-main {
        padding: 10px;
    }

    .layout-copy {
        text-align: center;
        padding: 10px 0 20px;
        color: #9ea7b4;
    }
</style>