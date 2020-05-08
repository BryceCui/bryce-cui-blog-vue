<template>
    <el-card class="card-component" shadow="always">
        <div slot="header" :body-style="{ padding: '0px' }" class="card-header">
            <img src="https://wpimg.wallstcn.com/e7d23d71-cf19-4b90-a1cc-f56af8c0903d.png">
        </div>
        <p>这是卡片</p>
    </el-card>
</template>

<script>
    export default {
        name: "Home"
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
    .card-component {
        .card-header {
            position: relative;
            height: 220px;
            width: 400px;

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
    }
</style>
