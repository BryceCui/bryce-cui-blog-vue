<template>
    <!--    <div class="body">-->
    <el-card class="card-component" style="margin-left:8px;">
        <div slot="header" class="card-header">
            <img src="https://wpimg.wallstcn.com/e7d23d71-cf19-4b90-a1cc-f56af8c0903d.png">
        </div>
        <div style="position:relative;">
            <pan-thumb :image="avatar" class="panThumb"/>
        </div>
        <div>
            <p>华盛顿卡还是多好看
            </p>
        </div>
    </el-card>
    <!--    </div>-->
</template>

<script>
    import PanThumb from './components/index'

    export default {
        components: {PanThumb},
        name: "Home",
        data() {
            return {
                avatar: "https://wpimg.wallstcn.com/f778738c-e4f8-4870-b634-56703b4acafe.gif"
            }
        }
    }
</script>

<style lang="scss">
    .card-component {
        .el-card__header {
            padding: 0px !important;
        }
    }

</style>
<style lang="scss" scoped>
    /*.body {*/
    /*width: 100%;*/
    .card-component {

        .card-header {
            position: relative;
            width: 400px;
            height: 220px;
            img {
                width: 100%;
                height: 100%;
                transition: all 0.2s linear;
                &:hover {
                    transform: scale(1.2, 1.2);
                    filter: contrast(130%);
                }
            }
        }

        .panThumb {
            z-index: 100;
            height: 70px !important;
            width: 70px !important;
            position: absolute !important;
            top: -95px;
            float: right;
            left: 0px;
            border: 5px solid #ffffff;
            background-color: #fff;
            margin: auto;
            box-shadow: none !important;
            /deep/ .pan-info {
                box-shadow: none !important;
            }
        }
    }
</style>
