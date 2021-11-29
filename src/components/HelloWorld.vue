<template>

    <div>
        <div class="item">
            <div style="width: 30vw; height: 40vh; background: #ccc">
                <convenience-image alignment="max-center" :src-nor="shupin" :src-err="defaultImg"/>
            </div>
            显示中间最大面积
        </div>

        <br>

        <div class="item">
            <div style="width: 30vw; height: 40vh; background: #ccc">
                <convenience-image alignment="max-contain" :src-nor="shupin" :src-err="defaultImg"/>
            </div>
            等比缩放至最大面积
        </div>

        <br>
        <div class="item">
            <div class="container">
                <convenience-image src-nor="http://img15.3lian.com/2015/f2/8/d/96.jpg2" :src-err="defaultImg"/>
            </div>
            图片不存在
        </div>

        <div class="item">
            <div class="container">
                <convenience-image :src-nor="shupin" :src-err="defaultImg"/>
            </div>
            w&lth,居中
        </div>

        <div class="item">
            <div class="container">
                <convenience-image :src-nor="hengpin" :src-err="defaultImg"/>
            </div>
            w>h,居中
        </div>

        <br>
        <div class="item">
            <div class="container">
                <convenience-image alignment="left" src-nor="http://img15.3lian.com/2015/f2/8/d/96.jpg2" :src-err="defaultImg"/>
            </div>
            图片不存在
        </div>
        <div class="item">
            <div class="container">
                <convenience-image alignment="left" :src-nor="shupin" :src-err="defaultImg"/>
            </div>
            w&lth,左对齐
        </div>
        <div class="item">
            <div class="container">
                <convenience-image alignment="left" :src-nor="hengpin" :src-err="defaultImg"/>
            </div>
            w>h,左对齐
        </div>

        <br>
        <div class="item">
            <div class="container">
                <convenience-image alignment="top" src-nor="http://img15.3lian.com/2015/f2/8/d/96.jpg2" :src-err="defaultImg"/>
            </div>
            图片不存在
        </div>
        <div class="item">
            <div class="container">
                <convenience-image alignment="top" :src-nor="shupin" :src-err="defaultImg"/>
            </div>
            w&lth,上对齐
        </div>
        <div class="item">
            <div class="container">
                <convenience-image alignment="top" :src-nor="hengpin" :src-err="defaultImg"/>
            </div>
            w>h,上对齐
        </div>

        <br>
        <div class="item">
            <div class="container">
                <convenience-image alignment="top-left" src-nor="http://img15.3lian.com/2015/f2/8/d/96.jpg2" :src-err="defaultImg"/>
            </div>
            图片不存在
        </div>
        <div class="item">
            <div class="container">
                <convenience-image alignment="top-left" :src-nor="shupin" :src-err="defaultImg"/>
            </div>
            w&lth,上对齐左对齐
        </div>
        <div class="item">
            <div class="container">
                <convenience-image alignment="top-left" :src-nor="hengpin" :src-err="defaultImg"/>
            </div>
            w>h,上对齐左对齐
        </div>

    </div>

</template>

<script>
    export default {
        name: 'HelloWorld',
        props: {
            msg: String
        },
        data() {
            return {
                defaultImg: require('../assets/defaultImg.png'),
                hengpin: 'https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fup.enterdesk.com%2Fedpic_360_360%2F92%2F69%2F9d%2F92699dfebec7af164c81596afe4ff735.jpg&refer=http%3A%2F%2Fup.enterdesk.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1640757931&t=22a08c5d5f363bf76770d27d8aa4268c',
                shupin: 'https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fc-ssl.duitang.com%2Fuploads%2Fblog%2F201403%2F29%2F20140329145413_hw4HA.thumb.1000_0.jpeg&refer=http%3A%2F%2Fc-ssl.duitang.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1640757974&t=d30a0cf017455800c5e4da00f7d18feb'
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .item {
        padding-left: 10px;
        padding-right: 10px;
        display: inline-block;
    }

    .container {
        background: #ccc;
        width: 150px;
        height: 150px;
    }

</style>
