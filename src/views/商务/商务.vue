<style lang="scss" scoped>
    .one{
        margin: 15px 0;
    }
    .text-item{
        height:250px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-around;
        padding-top: 20px;
        margin-bottom: 20px;
        >*{
            display: block;
        }
    }
    .large-btn{
        padding-left:50px;
        padding-right:50px;
    }
    .banner{
        height: 180px;
        font-size: 40px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .bg-black{
        background: rgb(28, 27, 32);
        color: white;
    }
</style>
<template>
    <el-tabs v-model="tab">
        <el-tab-pane label="评测服务" name="1">
            <div class="flex row-around">
                <div class="flex-1 ui-border-right flex column column-row-center f14 one">
                    <img src="~./icons/ico1.png" style="height:80px;">
                    <div class="text-item">
                        <b class="f20">基础测评</b>
                        <span>4天关键维度切入</span>
                        <span>100项无死角测评</span>
                        <span>580个日夜研发测评模型</span>
                        <span>真人测评员全程实测</span>
                        <span>敏感信息诚信保护</span>
                    </div>
                    <span class="mt15">将给您带来价值</span>
                    <span class="ui-rmb f24 f-color-orange mb30">2000万</span>
                    <el-button @click="link" class="large-btn mb15">服务详情</el-button>
                    <el-button @click="link" class="large-btn ml0">商务专员</el-button>
                </div>
                <div class="flex-1 ui-border-right flex column column-row-center f14 one">
                    <img src="~./icons/ico2.png" style="height:80px;">
                    <div class="text-item">
                        <b class="f20">商业测评</b>
                        <span>228项测评点深入测评</span>
                        <span>手术刀是的剖析观察</span>
                        <span>顶尖博彩战略师主持</span>
                        <span>品牌重生指导</span>
                        <span>国防级信息隐私保护</span>
                    </div>
                    <span class="mt15">将给您带来价值</span>
                    <span class="ui-rmb f24 f-color-orange mb30">7000万</span>
                    <el-button @click="link" class="large-btn mb15">服务详情</el-button>
                    <el-button @click="link" class="large-btn ml0">商务专员</el-button>
                </div>
                <div class="flex-1 flex column column-row-center f14 one">
                    <img src="~./icons/ico3.png" style="height:80px;">
                    <div class="text-item">
                        <b class="f20">主题定制测评</b>
                        <span>一期提升品牌力</span>
                        <span>一键植入玩家心智</span>
                        <span>一次真正的行业亮剑</span>
                        <span>68家合媒全网分发</span>
                    </div>
                    <span class="mt15">将给您带来价值</span>
                    <span class="ui-rmb f24 f-color-orange mb30">500万/期</span>
                    <el-button @click="link" class="large-btn mb15">服务详情</el-button>
                    <el-button @click="link" class="large-btn ml0">商务专员</el-button>
                </div>
            </div>
        </el-tab-pane>
        <el-tab-pane label="品牌建设" name="2">
            <div class="banner bg-black">
                无品牌 无未来
            </div>
            <div class="flex row-around">
                <div class="flex-1 ui-border-right flex column column-row-center f14 one">
                    <img src="~./icons/ico1.png" style="height:80px;">
                    <div class="text-item">
                        <b class="f20">基础型</b>
                        <span>品牌分析挖掘</span>
                        <span>主题策划专刊</span>
                        <span>精选18家合媒分发</span>
                    </div>
                    <span class="mt15">将给您带来价值</span>
                    <span class="ui-rmb f24 f-color-orange mb30">2000万</span>
                    <el-button @click="link" class="large-btn mb15">服务详情</el-button>
                    <el-button @click="link" class="large-btn ml0">商务专员</el-button>
                </div>
                <div class="flex-1 ui-border-right flex column column-row-center f14 one">
                    <img src="~./icons/ico2.png" style="height:80px;">
                    <div class="text-item">
                        <b class="f20">专业型</b>
                        <span>主题策划专刊</span>
                        <span>视频策划专刊</span>
                        <span>产品无缝植入</span>
                        <span>核心38家合媒分发</span>
                    </div>
                    <span class="mt15">将给您带来价值</span>
                    <span class="ui-rmb f24 f-color-orange mb30">7000万</span>
                    <el-button @click="link" class="large-btn mb15">服务详情</el-button>
                    <el-button @click="link" class="large-btn ml0">商务专员</el-button>
                </div>
                <div class="flex-1 flex column column-row-center f14 one">
                    <img src="~./icons/ico3.png" style="height:80px;">
                    <div class="text-item">
                        <b class="f20">旗舰型</b>
                        <span>主题策划专刊</span>
                        <span>视频策划专刊</span>
                        <span>产品无缝植入</span>
                        <span>品牌视频露出</span>
                        <span>全网68家合媒分发</span>
                    </div>
                    <span class="mt15">将给您带来价值</span>
                    <span class="ui-rmb f24 f-color-orange mb30">500万/期</span>
                    <el-button @click="link" class="large-btn mb15">服务详情</el-button>
                    <el-button @click="link" class="large-btn ml0">商务专员</el-button>
                </div>
            </div>
            
        </el-tab-pane>
        <!-- <el-tab-pane label="广告合作" name="3">
            <div class="flex flex-wrap">
                <el-card v-for="(item,index) in 5" :key="index" class="m10">
                    <div class="flex column column-col-center column-row-center">
                        <span class="mb15">广告标题</span>
                        <ui-img url="http://p3.pstatp.com/list/190x124/2ee00002a5277f829a38" style="width:200px;height:170px;"></ui-img>
                        <el-button class="block mt15 auto-center">商务专员</el-button>
                    </div>
                </el-card>
            </div>

            <div class="p40 pl50 pr50 m10 bg-black">
                <div class="mb15">溶解式广告</div>
                <div class="f28 mb20">像糖溶解在水里，像雨落进河流</div>
                <div>溶解式广告使您的广告与我们的产品无缝相容，完美结合。 <el-button type="text">联系商务专员</el-button></div>
            </div>
        </el-tab-pane> -->
    </el-tabs>
</template>

<script>
    export default {
        data () {
            return {
                tab:'1'
            }
        },
        methods:{
            link(){
                this.$alert('敬请期待')
            }
        },
    }
</script>