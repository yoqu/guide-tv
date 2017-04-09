<template>
    <div class="thumbnail">
        <a :href="zbInfo.url" target="_blank" class="live-vedio-screenshot">
            <!--<a data-id="http://star.longzhu.com/haiwang" data-name="海王Seaking" target='_blank' class="live-vedio-screenshot" style="cursor: pointer; height: 135px;">-->
            <div style="width: 100%; height: 135px;">
                <img alt="top1tv" :src="zbInfo.previewImg" target="_blank" :title="zbInfo.title" class="lazy"
                     style="width: 100%; height: 100%;">
            </div>
            <div class="live-flag">{{zbInfo.platform}}&nbsp;&nbsp;&nbsp;&nbsp;{{zbInfo.type}}</div>
        </a>
        <div class="caption">
            <div class="live-vedio-tit">{{zbInfo.title}}</div>
            <div class="mt10">
                <span class="pull-left">
                    <Icon type="ios-play"></Icon>
                    <span class="color-888">{{zbInfo.viewCount}}</span>
                </span>
                <div class="pull-right live-username slh">
                    <Icon type="person"></Icon>
                    <span class="color-888" :title="zbInfo.author">{{zbInfo.author}}</span>
                </div>
                <div class="clearfix"></div>
            </div>
        </div>
    </div>
</template>
<script>
    export default{
        props:['zbInfo'],
        data(){
            return {
                zbInfo: {
                    url: "http://star.longzhu.com/haiwang",
                    previewImg: "http://img2.plures.net/live/screenshots/394548/d776/96ac/46af/ca60/12dc/e55a/9d58/6fb2_1491702291.jpg",
                    title: "海王 宇宙第一全能王!",
                    platform: "龙珠",
                    type: "英雄联盟",
                    viewCount: 49991,
                    author: "海王Seaking"
                }
            };
        }
    }
</script>
<style>
    .thumbnail {
        display: block;
        padding: 4px;
        margin-bottom: 20px;
        line-height: 1.42857143;
        background-color: #fff;
        border: 1px solid #ddd;
        border-radius: 4px;
        -webkit-transition: border .2s ease-in-out;
        -o-transition: border .2s ease-in-out;
        transition: border .2s ease-in-out;
        margin-left:10px;
    }
    .live-vedio-screenshot{
        display: block;
        position: relative;
    }
    .live-vedio-tit{
        font-size:16px;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
        text-align: left;
    }
    .thumbnail .caption {
        padding: 9px;
        color: #333;
    }
    .live-flag {
        position: absolute;
        bottom: 0;
        width: 100%;
        height: 20px;
        color: #f4645f;
        text-align: right;
        padding-right: 10px;
        font-size: 12px;
        line-height: 20px;
        background-color: #000;
        filter: alpha(opacity=70);
        -moz-opacity: 0.7;
        -khtml-opacity: 0.7;
        opacity: 0.7;
    }
    .pull-left{
        float: left;
    }
    .pull-right{
        float: right;
    }
    .clearfix{
        clear: both;
    }
    .mt10 {
        margin-top: 10px;
    }
</style>