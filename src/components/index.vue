<template>
  <div>
<!--    展示轮播图-->
    <div class="swiper-container" id="swiper1">
        <ul>
            <li :class="indexLunBo==0?'activeLunBo':''" @mouseenter="tabLunBo(0)">服务领域 <span v-show="indexLunBo==0"></span></li>
            <li :class="indexLunBo==1?'activeLunBo':''" @mouseenter="tabLunBo(1)">服务网络 <span v-show="indexLunBo==1"></span></li>
            <li :class="indexLunBo==2?'activeLunBo':''" @mouseenter="tabLunBo(2)">我们的优势 <span v-show="indexLunBo==2"></span></li>
            <li :class="indexLunBo==3?'activeLunBo':''" @mouseenter="tabLunBo(3)">成功案例 <span v-show="indexLunBo==3"></span></li>
        </ul>
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <div class="lunBo" style="background-image: url('http://images.gshxkj.com.cn:8090/index/banner1.jpg');">
          </div>
        </div>
<!--        <div class="swiper-slide">-->
<!--          <div class="lunBo" style="background-image: url('http://images.gshxkj.com.cn:8090/index/banner2.jpg');">-->

<!--          </div>-->
<!--        </div>-->
        <div class="swiper-slide">
          <div class="lunBo" style="background-image: url('http://images.gshxkj.com.cn:8090/index/banner4.png');">

          </div>
        </div>
        <div class="swiper-slide">
          <div class="lunBo" style="background-image: url('http://images.gshxkj.com.cn:8090/index/banner8.png');">

          </div>
        </div>

        <div class="swiper-slide">
          <div class="lunBo" style="background-image: url('http://images.gshxkj.com.cn:8090/index/banner3.png');">
          </div>
        </div>

      </div>
      <div class="swiper-pagination swiper-pagination-white"></div>
      <div class="swiper-button-prev swiper-button-white" style="margin-left: 15px;"></div>
      <div class="swiper-button-next swiper-button-white" style="margin-right: 15px;"></div>
    </div>


<div class="contnet_height">

<!--      业务范围-->
      <div class="content" v-show="indexLunBo==0" >
      <el-row>
        <el-col :span="10">
          <div class="cc_left">
            <img src="http://images.gshxkj.com.cn:8090/index/ywfl_left.png" alt="">
          </div>
        </el-col>
        <el-col :span="14">
          <div>
            <div class="fwly" style="width: 100%;">
              业务范围
            </div>
            <el-row class="ywfw" >
              <el-col :span="6">
                <div>
                  <div class="ywfw_every">
                    <img src="http://images.gshxkj.com.cn:8090/index/ywfw1.png" alt="">
                  </div>
                  <p>产品及解决方案</p>
                </div>
              </el-col>
              <el-col :span="6">
                <div>
                  <div class="ywfw_every">
                    <img src="http://images.gshxkj.com.cn:8090/index/ywfw2.png" alt="">
                  </div>
                  <p>智慧司法</p>
                </div>
              </el-col>
              <el-col :span="6">
                <div>
                  <div class="ywfw_every">
                    <img src="http://images.gshxkj.com.cn:8090/index/ywfw3.png" alt="">
                  </div>
                  <p>系统集成</p>
                </div>
              </el-col>
              <el-col :span="6">
                <div>
                  <div class="ywfw_every">
                    <img src="http://images.gshxkj.com.cn:8090/index/ywfw4.png" alt="" style="width: 110px;">
                  </div>
                  <p>IT运维服务及其他</p>
                </div>
              </el-col>
            </el-row>
          </div>
        </el-col>
      </el-row>
    </div>

      <!--      服务网络-->

      <div class="content fwwl" v-show="indexLunBo==1" >
            <div>
                <div class="fwwl_left">
                    <img src="http://images.gshxkj.com.cn:8090/index/chinaMap.png" alt="">
                </div>
                <div class="fwwl_right">
                    <div>【客户分布图】</div>
                    <div>公司业务范围目前涵盖甘肃省12个地级市:兰州市、嘉峪关市、金昌市、白银市、天水市、武威市、张掖市、平凉市、酒泉市、庆阳市定西市、陇南市，并辐射西北五省（甘肃、陕西、宁夏、青海、新疆）。 大量企业、高校、市县两级政府部门都在与我公司的业务往来中受益匪浅，加速推进了信息化管理，提高了政府办事效率。</div>
                </div>
            </div>
      </div>

      <!--      我们的优势-->
      <div class="content" v-show="indexLunBo==2" style="padding: 40px 0 20px;">
        <el-row :gutter="20" class="mySuccess">
          <el-col :span="6">
            <div style="background-image: url('http://images.gshxkj.com.cn:8090/index/mySuccess.png')">
              <h6>丰富的行业经验</h6>
              <p>涉及领域广泛，已成功完成众多项目,满足了不同行业IT需求。</p>
            </div>
          </el-col>
          <el-col :span="6">
            <div style="border: 1px solid #A6C1DC;border-radius: 10px;height: 203px;margin-top: 8px;">
              <h6 style="margin-top: 21px;">完善的管理</h6>
              <p>专业成熟的项目管理、产品管理、IT服务管理以及供应商管理体系，保证每一个项目成功实施。</p>
            </div>
          </el-col>
          <el-col :span="6">
            <div style="border: 1px solid #A6C1DC;border-radius: 10px;height: 203px;margin-top: 8px;">
              <h6 style="margin-top: 21px;">专业的技术团队支持</h6>
              <p>拥有多行业、多品类专业技术人员，跟随时代脚步，掌握行业先进技术，高效率、高质量完成每一个项目。</p>
            </div>
          </el-col>
          <el-col :span="6">
            <div style="background-image: url('http://images.gshxkj.com.cn:8090/index/mySuccess.png')">
              <h6>先进的管理理念</h6>
              <p>
                公司顺应国家发展趋势，紧跟互联网发展步伐，始终以技术为核心，以科技创新为指引,为每位用户提供安全、快捷、高效、实用的专业信息化服务。
              </p>
            </div>
          </el-col>
        </el-row>
      </div>
<!--    成功案例-->
        <div class="content success" :style="{opacity:(indexLunBo==3)?'1':'0'}">
            <success></success>
        </div>
</div>

<!--      新闻模块-->
      <div class="news">
          <div>
            <p>新闻中心  <span>NEWS</span></p>
              <router-link :to="{ path: '/news',query:{num:0}}" tag="button"  >了解更多 ></router-link>
<!--              <button>了解更多 ></button>-->
          </div>
          <div>
              <marquee direction="up" behavior="scroll" scrollamount="2"  loop="-1"  height="100%"  hspace="10" vspace="10"  onmouseover="this.stop()" onmouseout="this.start()">
                  
                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:15}}" tag="p">环讯科技中标甘肃银行网络安全服务项目<span>2020-06-12</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:16}}" tag="p">环讯科技研发预售房交易资金监管平台<span>2020-06-12</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:1,detaiNum:9}}" tag="p">学习时报发表评论员文章：为维护人民健康提供有力法治保障<span>2020-06-12</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:18}}" tag="p">实战 | 便民缴税服务推动金融与民生互联互通<span>2020-06-12</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:19}}" tag="p">李兆云：软件产品质量管理的数字化转型<span>2020-06-12</span></router-link>


                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:14}}" tag="p">环讯科技正式开通400服务热线<span>2020-05-29</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:1,detaiNum:8}}" tag="p">特殊时期的全国两会，立起中国笃定前行的路标<span>2020-05-29</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:16}}" tag="p">分布式数据库在金融行业的应用和展望<span>2020-05-29</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:17}}" tag="p">实战 | 银行远程办公创新与实践<span>2020-05-29</span></router-link>

                  <router-link :to="{ path: '/news',query:{num:4,detaiNum:4}}" tag="p">表扬信——致玉门市住宅维修资金数据迁移小组<span>2020-05-22</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:1,detaiNum:7}}" tag="p">政府工作报告 ——2020年5月22日在第十三届全国人民代表大会第三次会议上<span>2020-05-22</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:14}}" tag="p">观点 |​ 建立中国金融业软件测试标准的探索<span>2020-05-22</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:15}}" tag="p">实战 | 移动云测试平台建设的实践与展望<span>2020-05-22</span></router-link>


                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:12}}" tag="p">赵克斌副总经理赴庆阳推进住宅维修资金项目<span>2020-05-15</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:1,detaiNum:6}}" tag="p">兰州高新区召开党工委（扩大）会议传达学习党中央和省、市有关会议精神安排高新区贯彻落实工作<span>2020-05-15</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:12}}" tag="p">【交通银行线上金融业务中心总裁 李豪】打造有温度的“零接触”金融服务<span>2020-05-15</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:13}}" tag="p">思想汇 | 金融科技的光荣与梦想<span>2020-05-15</span></router-link>

                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:11}}" tag="p">环讯科技与建设银行共同建设长庆油田职工食堂电子缴费系统<span>2020-04-27</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:1,detaiNum:5}}" tag="p">确保人民群众在国家治理中的主体地位<span>2020-04-27</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:11}}" tag="p">央行科技司李伟：落实发展规划 推动金融科技惠民利企<span>2020-04-27</span></router-link>



                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:10}}" tag="p">环讯科技与农业银行签订技术服务协议，联合建设住宅维修资金云管理平台<span>2020-04-20</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:4,detaiNum:3}}" tag="p">表扬信<span>2020-04-20</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:1,detaiNum:3}}" tag="p">科学精准施策确保疫情防控和经济社会发展双胜利<span>2020-04-20</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:1,detaiNum:4}}" tag="p">脱离业务模型的基础架构没有灵魂，金融行业IT双模建设我们该如何应对？ | 2020年度策划<span>2020-04-20</span></router-link>


                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:9}}" tag="p">润通集团调研环讯科技取得圆满成功<span>2020-04-12</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:1,detaiNum:2}}" tag="p">中国疫情防控彰显党的体制优势<span>2020-04-12</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:10}}" tag="p">观点 | 区块链技术对商业银行的影响分析及启示<span>2020-04-12</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:9}}" tag="p">观点 | 移动办公应用思考与风险控制<span>2020-04-12</span></router-link>




                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:8}}" tag="p">环讯科技助力甘肃金融企业创新发展<span>2020-04-03</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:6}}" tag="p">实战 | 新一代信息系统工程建设<span>2020-04-03</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:7}}" tag="p">实战丨金融科技创新赋能智慧旅游<span>2020-04-03</span></router-link>

                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:5}}" tag="p">深度 | 新基建投资领域与前景展望<span>2020-03-25</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:7}}" tag="p">兰州市高新区人社局莅临环讯科技关怀疫情期间企业复工复产并慰问企业职工<span>2020-03-23</span></router-link>

                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:5}}" tag="p">聚焦创业典型|兰州高新区优秀孵化企业 抓防控抓生产别样红（一）<span>2020-03-13</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:6}}" tag="p">聚焦创业典型|兰州高新区优秀孵化企业 抓防控抓生产别样红（二）<span>2020-03-13</span></router-link>

                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:4}}" tag="p">喜报传来开门红，再接重任显壮志 ——记甘肃环讯信息科技有限公司重大服务合同成功签约<span>2020-03-12</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:4,detaiNum:2}}" tag="p">远程办公，同心战疫情 <span>2020-03-07</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:4}}" tag="p">银行自动化运维项目建设八大难点问题解析 <span>2020-03-07</span></router-link>

                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:1}}" tag="p">甘肃环讯收到中共兰州高新技术产业开发区工作委员会的感谢信 <span>2020-03-01</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:1}}" tag="p">拥抱数字化时代，构建大数据体系 <span>2020-03-01</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:4,detaiNum:1}}" tag="p">战胜疫情，匹夫有责--甘肃环讯复工纪实 <span>2020-03-01</span></router-link>

                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:2}}" tag="p">勇于突破，开拓进取，积极投身于甘肃省信息化建设 <span>2020-03-01</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:3,detaiNum:3}}" tag="p">兰州高新区孵化企业通过ISO系列认证，为可持续创新研发奠定基础 <span>2020-03-01</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:1,detaiNum:1}}" tag="p">习近平：全面提高依法防控依法治理能力 为疫情防控提供有力法治保障 <span>2020-03-01</span></router-link>
                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:3}}" tag="p">守正创新 以金融科技磨砺核心竞争力 <span>2020-03-01</span></router-link>
<!--                  <router-link :to="{ path: '/news',query:{num:2,detaiNum:2}}" tag="p">《上海中医药杂志》向全国介绍中医治疗新型冠状病毒肺炎的甘肃经验 <span>2020-03-01</span></router-link>-->

              </marquee>

          </div>

      </div>
      <div class="jbx"></div>
<!--      服务热线-->
      <div class="content fwrx">
          <h5><span>服务热线</span><img src="@/assets/images/phone.png" ><span>0931-8121096</span></h5>
      </div>

  </div>
</template>

<script>
    import success from './success';
  import Swiper from "swiper"
export default {
  name: 'index',
    components:{
        success
    },
  data(){
    return{
      index:0,
      num:0,
      indexLunBo:0,
    }
  },
  methods:{
    dongxiao(index){
      this.index=index;
    },
    tabLunBo(index){
      this.indexLunBo=index;

    }
  },
  mounted: function () {
      var mySwiper = new Swiper('#swiper2', {
          autoplay: 3000,//可选选项，自动滑动
          freeMode : false,
      })
          var mySwiper = new Swiper('#swiper1', {
              autoplay : 3000,
              loop : true,
              pagination : '.swiper-pagination',
              prevButton:'.swiper-button-prev',
              nextButton:'.swiper-button-next',
              paginationClickable :true,
              effect : 'fade',
              autoplayDisableOnInteraction:false,
              preventLinksPropagation:true
      })

  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @import "../../node_modules/swiper/dist/css/swiper.css";
  .jbx{
      width: 1196px;
      margin: 0 auto;
      height: 1px;
      background: linear-gradient(to right,#fff,#C3C3C3,#fff);
  }
  .news{
      width:1196px;
      margin: 0 auto 51px;
      display: flex;
      height: 143px;
      box-shadow: 0 2px 12px 0 rgba(0,0,0,.2);
      div{
          box-sizing: border-box;
          display: flex;
          flex-direction: column;
          justify-content: center;
          align-items: center;
      }
      &>div:first-child{
          flex: 0.58;
          p{
              color: #10538F;
              font-size: 20px;
              span{
                  color:#FB3434;
                  font-size: 12px;
              }
          }
          button{
              outline: none;
              width: 130px;
              height: 32px;
              background: #58A4E7;
              color: #FFFEFE;
              font-size: 14px;
              border: none;
              border-radius: 16px;
              margin-top: 18px;
          }
      }
      &>div:nth-of-type(2){
          flex: 1.7;
          align-items: flex-start;
          p{
              cursor: pointer;
              padding-left: 73px;
              position: relative;
              color: #666666;
              font-size: 16px;
              margin-bottom: 16px;
              &:last-child{
                  margin-bottom: 0;
              }
              &:before{
                  position: absolute;
                  content: '';
                  display: block;
                  width: 8px;
                  height: 8px;
                  border-radius: 50%;
                  background: #58A4E7;
                  left: 34px;
                  top: 7px;
              }
              span{
                  float: right;
                  margin-right: 12px;
              }
          }
      }

  }
  .contnet_height{
      position: relative;
      height: 350px;
      display: flex;
      align-items: center;
  }
  .success{
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      margin: 0 auto;
  }
  .mySuccess{
    .el-col{
      div{
        box-sizing: border-box;
        overflow: hidden;
        padding: 0 20px;
        height: 220px;
        background-size: 100% 100%;
        background-repeat: no-repeat;
        h6{
          color: #009C8C;
          text-align: center;
          font-size: 16px;
          margin: 30px 0 15px;
        }
        p{
          font-size: 13px;
          color: #333;
          line-height: 30px;
        }
      }
    }
  }
.fwwl{
    background-image: url("http://images.gshxkj.com.cn:8090/index/fwwl_bg.png");
    background-size: 100% 100%;
    background-repeat: no-repeat;
    padding:10px 0;
    div{
        display: flex;
        .fwwl_left{
            flex: 1;
            img{
                display: block;
                margin: 0 auto;
            }
        }
        .fwwl_right{
            flex: 1.4;
            display: flex;
            div:first-child{
                flex: 1;
                -webkit-writing-mode: vertical-rl;
                writing-mode: vertical-rl;
                display: flex;
                align-items: center;
                justify-content: center;
                color: #7788B2;
                font-size: 15px;
            }
            div:last-child{
                padding: 0 20px 0 10px;
                color: #656565;
                font-size: 14px;
                line-height: 35px;
                flex:5;
                display: flex;
                align-items: center;
            }
        }
    }
}
  .fwrx{
      padding: 15px 0;
      h5{
          font-weight: 400;
          font-size: 18px;
          color: #A2A0A0;
          text-align: center;
          img{
              width: 21px;
              vertical-align: bottom;
          }
          span{
              margin: 0 7px;
          }
      }
  }
  .swiper-pagination{
    box-sizing: border-box;
    padding-right: 150px;
    margin-bottom: 70px;
    display: flex;
    justify-content: flex-end;
  }
  .ywfw{
    .ywfw_every{
      height: 100px;
      img{
        width: 70px;
        display: block;
        margin: 0 auto;
      }
    }
    div{
      padding-top: 15px;
      p{
        color: #1277E0;
        text-align: center;
      }
    }
  }
  .cc_left{
    padding-bottom: 20px;
    img{
      width: 414px;
    }
  }
  .swiper-container{

      position: relative;
      height: 500px;

      ul{
          position: absolute;
          z-index: 9999;
          width: 1196px;
          margin: 0 auto;
          bottom: 25px;
          left: 0;
          right: 0;
          li{
              background:rgba(255,255,255,1);
              opacity: 0.5;
              padding: 8px 0;
              width: 24%;
              margin-right: 1%;
              color: #39393A;
              height: 23.5px;
              text-align: center;
              float: left;
              cursor: pointer;
              span{
                  display: block;
                  width: 0;
                  height: 0;
                  border-style: solid;
                  border-width: 15px 15px 0 15px;
                  border-color: #1241CE transparent transparent transparent;
                  margin: 10px auto 0;
              }
          }
          .activeLunBo{
              background: #1241CE;
              color: #fff;
              opacity: 0.6;
          }
          z-index: 9999;
      }

  }

  .evenyList{
    overflow: hidden;
    padding-bottom: 50px;
    background-size: 100% 100%;
    background-repeat: no-repeat;
    transition: All 1s ease-in-out;
    -webkit-transition: All 1s ease-in-out;
    -moz-transition: All 1s ease-in-out;
    -o-transition: All 1s ease-in-out;
    div:first-child{
      height: 73px;
      margin-top: 40px;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    p{
      text-align: center;
      color: #fff;
    }
  }

  .lunBo{
    width: 100%;
    height: 100%;
    background-position:center;
    background-repeat:no-repeat;
    display: flex;
    flex-direction: column;
    justify-content: center;
    h1{
      color: #FBFCFD;
      font-size: 40px;
      font-weight: normal;
      letter-spacing: 2px;
      text-align: center;
      margin-bottom: 10px;
      span{
        color: #F4DF21;
      }
    }
  }
  .content{

    box-sizing: border-box;
    width: 1196px;
    margin:0 auto;
    &>p{
      text-align: center;
      color: #FFCC99;
      font-size: 18px;
      span{
        color: #666666;
        font-size: 15px;
      }
    }
  }
  .fwly{
    color: #666699;
    font-size: 28px;
    width: 422px;
    height: 36px;
    margin: 0 auto;
    text-align: center;
    background-image: url(http://images.gshxkj.com.cn:8090/index/icon4@2x.png);
    background-size: 100% 20%;
    background-repeat: no-repeat;
    background-position-y: bottom;
    padding: 10px 0;
  }

</style>
