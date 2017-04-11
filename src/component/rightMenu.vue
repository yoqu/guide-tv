<template>
    <Card class="right-menu-content">
        <p slot="title" class="title">
            <Icon type="ios-body"></Icon>
            {{title}}
        </p>
        <ul>
            <li v-for="(item,index) in users">
                <em class="title">{{index+1}}</em>  <a :href="item.url" target="_blank">{{ item.name }}</a>
            </li>
        </ul>
    </Card>
</template>
<script>
    export default {
        props: ["users", "title"],
        data () {
            return {}
        },

    }
</script>

<style>
    .right-menu-content ul li{
        list-style: none;
        margin-bottom: 5px;
        font-size: 14px;
        display: block;
        text-align: left;
    }
    .right-menu-content li em{
        color: #f2592a;
        margin-right:10px;
    }
    .right-menu-content .title{
        text-align: left;
    }
</style>