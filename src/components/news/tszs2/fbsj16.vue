<template>
    <div class="content_news">
        <div class="header">
            <h5>分布式数据库在金融行业的应用和展望</h5>
            <p class="biaoshu_time">发布时间：  2020-05-29     16:30:16</p>
        </div>
        <div class="main_news">

            <p>数据库技术作为应用系统的重要组成部分，从其出现开始就逐渐占据核心位置，目前几乎所有的计算机应用都无法离开数据库系统的底层支撑，金融行业尤其如此。金融互联网化的迅速发展要求金融数据库系统同时具备高性能、可扩展、高可用和高容错特性，传统数据库管理系统难以同时满足这些特性。为了应对金融互联网化带来的挑战，分布式数据库系统逐渐成了金融行业的选型方案。对此，本文将对分布式数据库在金融行业的发展进行深入的分析和探讨。 </p>
            <p class="new_title">一、数据库技术发展历史和分布式数据库的现状 </p>
            <p>数据库技术发源于20世纪60年代，是一种通过高效自动化方式实现数据信息管理的技术手段，其出现奠定了一个新的计算机科学分支。随着计算机技术的广泛应用，数据库技术在计算机应用领域也变得原来越重要，目前几乎所有的计算机应用都离不开数据库系统的支撑，数据库成为数据处理的主要技术手段。</p>
            
            <p>数据库的主要目的是实现对数据的有效管理，即实现对数据的分类、组织、编码、存储、检索和有效维护。随着软硬件技术的不断发展，数据库技术也有了长足进步。从数据管理的方式来看，数据库技术经历了人工管理、文件系统和数据库系统等多个阶段。</p>
            <p>（一）数据库技术的形成过程</p>
            <p>数据模型是数据库系统的核心，在数据模型发展的不同阶段，数据库技术也经历了以下3个发展阶段。</p>
            <p>1. 层次模型和网状数据库管理系统</p>
            <p>这个阶段的主要代表是IBM公司在1969年研制的层次模型数据库管理系统。层次数据模型是整个数据库系统的先驱，而网状数据库则奠定了完整的数据库概念、方法和技术。</p>


            <p>2. 关系数据库管理系统（RDBMS）</p>
            <p>IBM公司的研究员E.F.Codd在题为《大型共享数据库数据的关系模型》的论文中提出了数据库的关系模型，为关系数据库技术奠定了理论基础。在后来开发的各种数据库系统中，关系型数据库几乎成了垄断的态势。目前，虽然有各种新的数据库形式出现，但关系型数据库依然在使用范围上占据了领导地位。</p>
            <p>IBM在发布这一理论后，首先在自有的OS/390进行实现，当下还有大量的金融机构使用OS/390支撑关键业务系统运行。</p>
            <p>真正使关系数据库技术实用化的关键人物是James Gray。Gray在解决如何保障数据的完整性、安全性、并发性以及数据库的故障恢复能力等重大技术问题方面发挥了关键作用。关系数据库系统的出现，促进了数据库的小型化和普及化。</p>
            <p>基于以上技术进步，Oracle打造了基于开放系统的Oracle数据库系统。Oarcle数据库系统的高速商业化发展，奠定了其在关系型数据库领域的霸主地位。</p>
            <p>3. 新一代数据库技术的研究和发展</p>
            <p>计算机技术的进一步发展，伴随很多关系型数据库处理起来捉襟见肘的问题，在这样的背景下，新一代的数据库应运而生。下面从数据模型、新技术内容、应用领域3个方面来阐述新一代数据库系统的发展方向。</p>
            <p>（1）面向对象的方法和技术对数据库发展的影响</p>
    
            <p>随着面向对象的方法和技术的出现，数据库技术也迎来了新的发展。数据库逐渐利用面向对象的方法和技术，建立了面向对象的数据库模型（简称对象模型），主要是在传统的RDBMS进行不同层次的扩充，如建立对象关系（OR）模型和建立对象关系数据库（ORDB）。</p>
            <p>（2）数据库技术与多学科技术的深入结合</p>
            <p>数据库技术与多学科技术的有机结合是当前数据库发展的重要特征。计算机领域中其他新兴技术的发展对数据库技术产生了重大影响，传统的数据库技术和其他计算机技术的结合、互相渗透，使数据库不断涌现新的技术内容。数据库的许多概念、技术内容、应用领域，甚至某些原理都有了重大的发展和变化，促使建立和实现了一系列新型的数据库，如分布式数据库、并行数据库、演绎数据库、知识库、多媒体库、移动数据库等。</p>
            <p>（3）面向专门应用领域的数据库技术不断产生</p>
            <p>为了适应数据库应用多元化的要求，在传统数据库基础上，结合特有应用领域和场景，研究适合该领域的特殊数据库技术，加强了数据库技术在特定角度的发展，出现了工程数据库、统计数据库、科学数据库、空间数据库、地理数据库、Web数据库等，这是当前数据库技术发展的又一重要特征。</p>
            <p>（二）分布式数据库的分类</p>
            <p>应用对数据库处理能力的要求越来越高，集中式数据库已无法满足数据处理的要求，需要更多的处理单元参与到数据的处理中来。为了应对这种处理要求，分布式数据库应运而生，并成为传统集中数据库的一个重复分支。</p>
            <p>分布式数据库从数据的分布实现上分为以下3类：</p>
            <p>1. Sharding（分片式）</p>
            <p>在传统单机数据库上进行数据分片，通过业务层或中间路由层（Proxy）将不同的请求发送给不同的数据库实例。代表的方案有：业务层拆分，分库分表；基于Proxy的各类数据库中间件。分片是不得已而为之的行为，是由于单表达到了单节点处理的上限，需要通过分片的形式将处理要求进行分散。分片会为了满足数据库架构的要求而牺牲业务层的应用性能和灵活性。</p>
            <p>商用的基于分片的数据库有IBM的DB2DPF，开源的MySQL同样支持分片的数据库能力。</p>
            <p>2. Shared-everything（共享存储）</p>
            <p>在共享存储的模式下，又可以细分为SharedDisk和SharedLog。</p>
            <p>SharedDisk是将多个数据库引擎节点底层挂载在一个共享的存储系统上，所有的数据库引擎都可以看到所有数据，在多个数据库引擎实例之前加载一个类似负责均衡的数据库代理层，将数据库负载分布到不同的引擎上，由于每个引擎都能看到所有数据，所以可以进行全量数据的处理，从而达到扩展整个数据库系统处理能力的目的。典型的商用产品有OracleRAC，DB2pureScale，开源的MySQL有MySQLonCeph，MySQLonClusterFS。这种方式可提高底层共享存储的能力，通过增加数据库引擎节点来实现数据库处理能力的提升，同时由于所有的数据都可见，在应用层面的兼容性也更好。</p>
            <p>SharedLog是近几年发展起来的技术。随着云计算技术的发展，出现了一些面向云端分布式存储设计的分布式数据库，提出了以数据库日志为核心的日志，即数据库的概念。通过利用分布式存储的优势，将数据库日志和分布式存储结合起来，实现数据库日志的一致性和高可用性，日志落地后其他数据再通过缓存逐渐落地，通过这种方式提高数据库的处理能力。代表的解决方案有AmazonAurora和MySQLGroupReplication。</p>
            <p>3. Shared-nothing（纯分布式架构）</p>
            <p>Shared-nothing是目前业界最新的全分布解决方案，具有单点、无中心、无限平等在数据库领域非常有利的特性，同时具备自动分片，无关联的请求没有公共的依赖路径，代表系统有GoogleSpanner/F1和TiDB。但目前产品在成熟度、性能和对应用的兼容性方面还都有局限性。</p>
            <p>（三）云原生数据库对分布式数据库发展的影响</p>
            <p>随着云计算技术的不断发展，“云原生”的概念应运而生。所谓云原生就是能够支持DevOps、持续交付（ContinuousDelivery）、微服务（MicroServices）、敏捷基础设施（AgileInfrastructure）、康威定律（ConwaysLaw）等云技术的实现方式。与云技术深度结合的云原生特点也给分布式数据库的发展带来了巨大的影响，利用云技术大规模、高性能，以及敏捷的基础设施和多租户的共享机制等特性，可使原来在传统条件下分布式数据库无法达到的能力得到有效扩充。典型的例子就包括AmazonAurora、腾讯CynosDB、阿里云PolarDB等，这些分布式数据库解决方案充分利用了云平台，尤其是公有云平台的底层能力，大大提高了单一用户的处理能力，基于分时、空间换时间和最终一致性等多方面的优化，使得基于云原生的分布式数据库产品成为未来数据库发展的重要趋势。 </p>
            <p class="new_title">二、金融行业对数据库的需求 </p>
            <p>（一）金融行业数据库的现状</p>
            <p>目前国内金融行业使用的数据库还是以传统的国外商用数据库产品为主，大致分为以下几种情况。</p>
            <p>1. 国有大型银行的数据库现状</p>
            <p>在国有大型银行中，以OS/390为代表的大型机能够达到一定数量的占比，与之匹配的是IBM专门为OS/390大型机定制的DB2数据库系统，数据库产品和操作系统、物理设备高度整合，具有良好的处理能力和可靠性，目前主要用于大型银行的核心银行系统。但由于造价昂贵，且目前全球范围内使用的客户逐渐减少，其技术发展的速度相对缓慢。同时，由于中国银行业务发展突飞猛进，尤其是互联网金融、移动支付等金融服务的爆炸式扩展，使得目前国内各大银行的大型机系统已经是全球最大规模的系统，整个系统的可靠性风险逐渐上升。</p>
            <p>2. 部分股份制银行、城商行、农商行的数据库现状</p>
            <p>在部分股份制银行、城商行、农商行中，由于历史原因还有大量基于AS400的IBMDB2数据库在使用，AS400上的DB2也是一个数据库产品、操作系统和物理设备高度整合的解决方案，开发性差。由于全球技术发展的趋势，AS400的市场占有率大幅下滑，从而造成了AS400的技术发展和支持都具有较大风险。</p>
            <p>3. 多数金融机构使用数据库的现状</p>
            <p>包括国有大型银行、股份制银行、城商行、农商行在内的众多金融机构，都在大量使用以小型机、高端x86服务器为硬件基础的Oracle，DB2等国外商用数据库。但受国际形势影响，使用这些产品具有很多潜在风险。</p>
            <p>4. 其他类型数据库的探索</p>
            <p>部分金融机构开始积极尝试包括自研、开源MySQL，PostgreSQL在内的各种数据库产品的探索。</p>
            <p>（二）金融行业数据库转型的潜在动力</p>
            <p>随着普惠金融、数字金融的快速推进，数据能力已经成为金融机构在新时代提升业务能力的重要抓手。与此同时，移动互联网和电子支付业务的蓬勃发展，给金融行业的典型应用场景，如核心账户与账务交易、在线支付/移动支付交易业务、实时交易监控与指标分析等，带来新数据形态下的金融系统能力需求。</p>
            <p>一是金融行业的数据急剧增长，对数据存储和管理提出了更高要求。以大型商业银行为例，通常拥有成百上千个业务系统以及上亿用户的海量数据，且数量呈现指数级增长，从TB级别增加到PB级。</p>
            <p>二是金融行业对业务连续性能力更加重视。金融行业对IT端安全可控要求不断提升，在确保数据不丢失的同时，还要做好数据的容灾备份以及核心数据系统的“双活”。在数据库运行的过程中，数据通过各种技术被实时同步到两个数据中心的数据库实例中，当一个中心发生故障时，业务可以及时地切换到另一个中心，从而实现业务的不间断运行。</p>
            <p>三是面临高并发业务和大用户量带来的系统压力。随着互联网金融业务的开展，金融行业用户量和用户自身的应用权限不断增加，持续面临高并发业务和大用户量带来的系统压力。如过去银行主要通过柜面接收账单查询，现在则依托移动端用户自助查询，在某一峰值的操作量就可能超过过去一整天业务操作量的总和。</p>
            <p>四是要求移动应用响应速度更快。在移动互联网用户应用需求迅速增加的背景下，用户对移动应用的响应速度也有了更高要求，移动端响应必须做到秒级以下。除此之外，金融行业自身也需要提升数据技术能力和业务价值，增强自身的运营管理能力。</p>
            <p>五是技术层面的国产化需求。随着贸易摩擦愈演愈烈，一系列的经济制裁和技术封锁使得自主可控变得越发迫切。金融业在稳定性和安全性上对数据产品的要求近乎严苛，所以急需能满足核心系统需求的真正国产自主数据库产品。</p>
            <p>六是整体拥有成本方面的考虑。由于数据处理量的大幅上升，如果继续采用原有的国外商用数据库产品，金融机构需承担巨额成本，而大量的成本压力将促使金融机构逐渐采用更加廉价有效的分布式数据库解决方案，逐步替代原有的国外传统商用产品。</p>
            <p>（三）金融行业进行分布式数据库转型的路径</p>
            <p>1. 注意事项</p>
            <p>金融行业已经大量使用了传统的集中式数据库模式，也已经具有了长期运维的经验，如何快速有效地实现从传统的集中式数据库到分布式数据库的转型，成为金融机构必须面对的问题。分布式数据库与传统的集中式数据库相比，有以下不同的特点，是金融行业进行转型过程中必须注意的。</p>
            <p>一是分布式数据库通过将数据库处理的要求分散到多个处理节点，来达到提高性能的目标，所以在金融行业原有的业务逻辑上要进行相应的适配。对业务系统进行分层解耦，确定应用层、服务层及数据层的边界，以适应系统弹性扩展的需求。</p>
            <p>二是分布式数据库要对数据进行分区，比如按照时间做Range分区、按照记录的某个特征值做Hash分区。保持每个分区的大小适中，才能更好地实现系统的负载均衡、调度以及扩展性。</p>
            <p>三是需要充分理解分布式数据库的工作逻辑，从业务上尽量利用分布式的并行处理能力，将不同的任务进行并行处理，从而提高整体效率。同时，还要理解分布式带来的是整体效率的提升，针对具体业务的处理逻辑在低负载的情况下不一定比原有的集中式数据库效率更高，所以要针对这个特性进行应用逻辑预期的调整。</p>
            <p>2. 规划建议</p>
            <p>从传统集中式向分布式过渡的过程中，建议考虑以下建设规划，从而确保过渡的可行性和可靠性。</p>
            <p>（1）先增量，后存量</p>
            <p>对于金融机构内互联网跨界融合等增量业务，因为对安全性要求较低，不会发生金融安全风险，可以先行替换试验。当新上线分布式事务数据库能满足业务需求，并且相关业务人员已适应相关操作方法和模式后，通过切割流量的方法逐步对存量的核心业务进行替换。在存量业务替换的同时，需要同时维护原系统的备份，作为灾备方案。当新系统稳定运行得到验证后，逐步下线原系统。</p>
            <p>（2）按业务性能瓶颈顺序</p>
            <p>分布式事务数据库带来强大的吞吐/处理能力，金融机构可对当前各类业务性能瓶颈进行分析评估，明确当前哪项指标急需分布式事务数据库方案进行解决，按照一定的优先级顺序，逐轮进行流量分割处理，在缓解现有业务压力的同时，验证新系统的各项能力，层层递进。</p>
            <p>（3）按不同业务的技术实现类型规划</p>
            <p>金融机构内的业务纷繁复杂，各类业务对信息系统的技术要求并不相同。如转账业务要求大并发的事务能力，批量计提结息业务要求大规模数据的并行处理能力，日志分析要求实时大规模的数据分析能力。所以金融机构可按照不同业务对技术的需求能力，安排改造顺序，从而逐步验证分布式事务数据库能力。</p>
            <p>（4）注重知识储备和传递</p>
            <p>分布式数据库在业界处于实践起步阶段。金融行业应用分布式数据库需要在实施阶段，首先进行深入的知识传递和过渡。</p>
        </div>
        <p class="next" @click="toParent">下一篇：实战 | 移动云测试平台建设的实践与展望</p>
    </div>
</template>

<script>
    export default {
        name: "newsDetail",
        methods:{
            toParent(){
                this.$emit('changeIndex',17)
            }
        }
    }
</script>

<style scoped lang="scss">
    .little_title{
        display: block;
        color: #333;
        text-align: left;
        font-weight: bold;
    }
    .image_describe{
        text-align: center;
        margin:10px 0;
        padding-left: 137px;
        color: rgba(0,0,0,.8)!important;
    }
    .new_title{
        text-align: center!important;
        color: rgba(0,0,0,.9)!important;
        font-size: 15px!important;
        font-weight: bold;
    }
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
        .biaoshu_time{
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
        span{
            color: #000;
            font-weight: bold;
        }
        img{
            display: block;
            margin: 0 auto 35px;
        }
    }
</style>