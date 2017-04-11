<template>
    <Row>
        <Col span="4" class="wrapper-container left-menu">
        <rightMenu :title="menus.title" :users="menus.users"></rightMenu>
        </Col>
        <Col span="15" class="zb-list wrapper-container">
        <Row type="flex" justify="start" class="code-row-bg">
            <Col span="6" v-for="zb in zbs">
            <viewBox :zb-info="zb"></viewBox>
            </Col>
        </Row>
        </Col>
        <Col span="4"  class="wrapper-container right-menu">
        <rightMenu :title="menus.title" :users="menus.users"></rightMenu>
        </Col>
    </Row>
</template>
<script>
    import viewBox from '../component/viewBox.vue';
    import rightMenu from '../component/rightMenu.vue'
    export default{
        data() {
            return {
                msg: "直播导航",
                menus: {
                    title: "主播排行榜",
                    users: [{
                        url:"http://www.baidu.com",
                        name:"文森特丶v1ncent"
                    },{
                        url:"http://www.baidu.com",
                        name:"文森特丶v1ncent"
                    },{
                        url:"http://www.baidu.com",
                        name:"文森特丶v1ncent"
                    },{
                        url:"http://www.baidu.com",
                        name:"文森特丶v1ncent"
                    },{
                        url:"http://www.baidu.com",
                        name:"文森特丶v1ncent"
                    },{
                        url:"http://www.baidu.com",
                        name:"文森特丶v1ncent"
                    },{
                        url:"http://www.baidu.com",
                        name:"文森特丶v1ncent"
                    },{
                        url:"http://www.baidu.com",
                        name:"文森特丶v1ncent"
                    },{
                        url:"http://www.baidu.com",
                        name:"文森特丶v1ncent"
                    },]
                },
                zbs: [{
                    url: "http://star.longzhu.com/haiwang",
                    previewImg: "http://img2.plures.net/live/screenshots/394548/d776/96ac/46af/ca60/12dc/e55a/9d58/6fb2_1491702291.jpg",
                    title: "海王 宇宙第一全能王!",
                    platform: "龙珠",
                    type: "英雄联盟",
                    viewCount: 49991,
                    author: "海王Seaking"
                }, {
                    url: "http://star.longzhu.com/haiwang",
                    previewImg: "http://img2.plures.net/live/screenshots/394548/d776/96ac/46af/ca60/12dc/e55a/9d58/6fb2_1491702291.jpg",
                    title: "海王 宇宙第一全能王!",
                    platform: "龙珠",
                    type: "英雄联盟",
                    viewCount: 49991,
                    author: "海王Seaking"
                }, {
                    url: "http://star.longzhu.com/haiwang",
                    previewImg: "http://img2.plures.net/live/screenshots/394548/d776/96ac/46af/ca60/12dc/e55a/9d58/6fb2_1491702291.jpg",
                    title: "海王 宇宙第一全王!",
                    platform: "龙珠",
                    type: "英雄联盟",
                    viewCount: 49991,
                    author: "海王Seaking"
                }, {
                    url: "http://star.longzhu.com/haiwang",
                    previewImg: "http://img2.plures.net/live/screenshots/394548/d776/96ac/46af/ca60/12dc/e55a/9d58/6fb2_1491702291.jpg",
                    title: "海王 宇宙第一全王!",
                    platform: "龙珠",
                    type: "英雄联盟",
                    viewCount: 49991,
                    author: "海王Seaking"
                }, {
                    url: "http://star.longzhu.com/haiwang",
                    previewImg: "http://img2.plures.net/live/screenshots/394548/d776/96ac/46af/ca60/12dc/e55a/9d58/6fb2_1491702291.jpg",
                    title: "海王 宇宙第一全王!",
                    platform: "龙珠",
                    type: "英雄联盟",
                    viewCount: 49991,
                    author: "海王Seaking"
                }, {
                    url: "http://star.longzhu.com/haiwang",
                    previewImg: "http://img2.plures.net/live/screenshots/394548/d776/96ac/46af/ca60/12dc/e55a/9d58/6fb2_1491702291.jpg",
                    title: "海王 宇宙第一全王!",
                    platform: "龙珠",
                    type: "英雄联盟",
                    viewCount: 49991,
                    author: "海王Seaking"
                }]
            }
        },
        components: {viewBox, rightMenu}
    }
</script>
<style>
    .code-row-bg {
        padding-left: 10px;
    }
    .zb-list{
        padding: 25px 25px 25px 0;
        margin: 30px auto 20px;
    }
    .right-menu{
        margin: 30px auto 20px 10px;
    }
    .left-menu{
        margin: 30px 10px 20px 0px;
    }
    .wrapper-container {
        margin-top:30px;
        background: #fff;
        border-radius: 6px;
    }
</style>