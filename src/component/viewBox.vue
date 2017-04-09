<template>
        <Card class="thumbnail grid">
            <a :href="zbInfo.url" target="_blank" class="live-vedio-screenshot">
                <!--<a data-id="http://star.longzhu.com/haiwang" data-name="海王Seaking" target='_blank' class="live-vedio-screenshot" style="cursor: pointer; height: 135px;">-->
                <figure class="effect-romeo" style="width: 100%; height: 135px;">
                    <img alt="top1tv" v-lazy="zbInfo.previewImg" target="_blank" :title="zbInfo.title" class="lazy"
                         style="width: 100%; height: 100%;">
                    <figcaption>
                        <h2><Icon type="eye"></Icon></h2>
                    </figcaption>
                </figure>
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
        </Card>
</template>
<script>
    export default{
        props:['zbInfo'],
        data(){
            return {

            };
        }
    }
</script>
<style>
    .thumbnail {
        display: block;
        margin-bottom: 20px;
        margin-left:20px;
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

    .grid figure {
        position: relative;
        display: inline-block;
        overflow: hidden;
        margin: -0.135em;
        background: #3085a3;
        text-align: center;
        cursor: pointer;
    }

    .grid figure img {
        position: relative;
        display: block;
        min-height: 100%;
        opacity: 0.8;
    }

    .grid figure figcaption {
        padding: 2em;
        color: #fff;
        text-transform: uppercase;
        font-size: 1.25em;
        -webkit-backface-visibility: hidden;
        backface-visibility: hidden;
    }

    .grid figure figcaption::before,
    .grid figure figcaption::after {
        pointer-events: none;
    }

    .grid figure figcaption,
    .grid figure a {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
    }

    /* Anchor will cover the whole item by default */
    /* For some effects it will show as a button */
    .grid figure a {
        z-index: 1000;
        text-indent: 200%;
        white-space: nowrap;
        font-size: 0;
        opacity: 0;
    }

    .grid figure h2 {
        word-spacing: -0.15em;

        font-weight: 300;
    }

    .grid figure h2 span {
        font-weight: 800;
    }

    .grid figure h2,
    .grid figure p {
        margin: 0;
    }

    .grid figure p {
        letter-spacing: 1px;
        font-size: 68.5%;
    }
    figure.effect-romeo {
        -webkit-perspective: 1000px;
        perspective: 1000px;
    }

    figure.effect-romeo img {
        -webkit-transition: opacity 0.35s, -webkit-transform 0.35s;
        transition: opacity 0.35s, transform 0.35s;
        -webkit-transform: translate3d(0,0,300px);
        transform: translate3d(0,0,300px);
    }

    figure.effect-romeo:hover img {
        opacity: 0.6;
        -webkit-transform: translate3d(0,0,0);
        transform: translate3d(0,0,0);
    }

    figure.effect-romeo h2,
    figure.effect-romeo p {
        margin-top: 20px;
        opacity: 0;
        -webkit-transition: opacity 0.35s, -webkit-transform 0.35s;
        transition: opacity 0.35s, transform 0.35s;
    }


    figure.effect-romeo:hover h2 {
        opacity: 1;
        -webkit-transform: scale(1);
        transform: scale(1);
    }

    figure.effect-romeo:hover p {
        opacity: 1;
        -webkit-transform: translate3d(0,0,0);
        transform: translate3d(0,0,0);
    }
</style>