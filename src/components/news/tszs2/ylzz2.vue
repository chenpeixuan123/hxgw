<template>
    <div class="content_news">
        <div class="header">
            <h5>《上海中医药杂志》向全国介绍中医治疗新型冠状病毒肺炎的甘肃经验 </h5>
            <p>发布时间：  2020-03-01     16:50:18</p>
        </div>
        <div class="main_news">
            <p>新型冠状病毒肺炎COVID-19爆发以来，甘肃省91例确诊病例中，有89例使用了中医药治疗，中医药治疗率达到了97.8%，治愈出院65例，治愈率为71.4%，治愈出院患者均全程使用中医药治疗,甘肃方剂在全国产生重大影响。为了将甘肃地区中医诊疗新冠肺炎的经验分享给全国临床一线的医护人员，《上海中医药杂志》特向甘肃省中医药防治新冠肺炎中医药专家组组长、甘肃省应对新型冠状病毒肺炎科研攻关特别专项专家组副组长张志明教授约稿并以《新型冠状病毒肺炎的中医临床特征与辨证论治—甘肃经验 》为题目刊发介绍宣传甘肃经验。</p>
            <p>甘肃新型冠状病毒肺炎感染率、临床症状、中医证候与东南省份均具有显著差异。具有明显过渡性特点，且由东南省区向西北省区呈阶梯形分布。结合地区气候、地域特征和临床观察，张志明教授团队认为新冠肺炎属于中医“温疫”范畴，具有流行性、传染性等特点，是以肺脏为主要病位的传染病，并在疫情的防控过程中极力推荐和支持中医药的使用，坚持中西医并重、各取所长的诊疗思路。古代中医特别是《温热论》、《温病条辨》等中医经典著作，为后世提供了很多宝贵有效的治疗温疫的临床实践经验。甘肃地区新型冠状病毒肺炎热郁的特征突出，即湿邪贯穿全病程，并有兼夹，但与武汉地区相比湿邪表现不太突出；化热较为迅速，且易于出现阳明脏腑证候。因此甘肃省的中医药诊治方案不应照搬国家方案而应根据本地的气候及患者特点，有针对性地制定防治方案。应针对不同时期不同个体不同的病理状态进行调节，从预防、治疗和预后三个环节进行个体化治疗，采用“一患一方案”进行全程跟进治疗，取得了明显的临床疗效，形成临床特征与辨证论治的甘肃经验。 </p>
            <p>新冠肺炎疫情暴发以来，甘肃应对疫情中医科研攻关团队在张志明教授的带领下，主导制定了《甘肃省新型冠状病毒感染肺炎中医药防治方案》，同时与西医专家组共同拟定了中西医结合救治方案，共同进行远程会诊、治疗，积极开展中药制剂筛选完善和临床验证推广，我省拟定的新冠肺炎预防方、治疗方、康复方和藏药方共计2.5万余剂已随第四批、第五批甘肃援助湖北医疗队送抵武汉，产生了积极的社会影响。</p>
        </div>
        <p class="next" @click="toParent">下一篇：守正创新 以金融科技磨砺核心竞争力</p>
    </div>
</template>

<script>
    export default {
        name: "newsDetail",
        methods:{
            toParent(){
                this.$emit('changeIndex',3)
            }
        }
    }
</script>

<style scoped lang="scss">
    .next{
        cursor: pointer;
        color: #095793;
        font-size: 14px;
        text-align: right;
        margin-bottom: 86px;
    }
    .header{
        margin-bottom: 35px;
        h5{
            color: rgba(1,1,1,.9);
            font-size: 20px;
            text-align: center;
            margin: 33px 0 12px;
        }
        p{
            height: 30px;
            line-height: 30px;
            text-align: center;
            font-size: 12px;
            color:rgba(1,1,1,.9);
            background: rgba(1,1,1,.05);
        }
    }
    .main_news{
        p{
            color: #666666;
            font-size: 14px;
            line-height: 31px;
            text-indent: 2em;
            margin-bottom: 25px;
        }
    }
</style>