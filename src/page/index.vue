<template>
    <div class="zb-list wrapper-container" >
        <Row type="flex" justify="start" class="code-row-bg">
            <Col span="5" v-for="zb in zbs">
                <viewBox :zb-info="zb"></viewBox>
            </Col>
        </Row>
    </div>
</template>
<script>
    import viewBox from '../component/viewBox.vue';
    export default{
        data() {
            return {
                msg: "直播导航",
                zbs:[{
                    url: "http://star.longzhu.com/haiwang",
                    previewImg: "http://img2.plures.net/live/screenshots/394548/d776/96ac/46af/ca60/12dc/e55a/9d58/6fb2_1491702291.jpg",
                    title: "海王 宇宙第一全能王!",
                    platform: "龙珠",
                    type: "英雄联盟",
                    viewCount: 49991,
                    author: "海王Seaking"
                },{
                    url: "http://star.longzhu.com/haiwang",
                    previewImg: "http://img2.plures.net/live/screenshots/394548/d776/96ac/46af/ca60/12dc/e55a/9d58/6fb2_1491702291.jpg",
                    title: "海王 宇宙第一全能王!",
                    platform: "龙珠",
                    type: "英雄联盟",
                    viewCount: 49991,
                    author: "海王Seaking"
                },{
                    url: "http://star.longzhu.com/haiwang",
                    previewImg: "http://img2.plures.net/live/screenshots/394548/d776/96ac/46af/ca60/12dc/e55a/9d58/6fb2_1491702291.jpg",
                    title: "海王 宇宙第一全王!",
                    platform: "龙珠",
                    type: "英雄联盟",
                    viewCount: 49991,
                    author: "海王Seaking"
                },{
                    url: "http://star.longzhu.com/haiwang",
                    previewImg: "http://img2.plures.net/live/screenshots/394548/d776/96ac/46af/ca60/12dc/e55a/9d58/6fb2_1491702291.jpg",
                    title: "海王 宇宙第一全王!",
                    platform: "龙珠",
                    type: "英雄联盟",
                    viewCount: 49991,
                    author: "海王Seaking"
                },{
                    url: "http://star.longzhu.com/haiwang",
                    previewImg: "http://img2.plures.net/live/screenshots/394548/d776/96ac/46af/ca60/12dc/e55a/9d58/6fb2_1491702291.jpg",
                    title: "海王 宇宙第一全王!",
                    platform: "龙珠",
                    type: "英雄联盟",
                    viewCount: 49991,
                    author: "海王Seaking"
                },{
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
        components:{viewBox}
    }
</script>
<style>
    .wrapper-container{
        background: #fff;
        width: 90%;
        margin: 30px auto 20px;
        border-radius: 6px;
        box-shadow: 0 1px 1px 0 rgba(0,0,0,.1);
    }
</style>