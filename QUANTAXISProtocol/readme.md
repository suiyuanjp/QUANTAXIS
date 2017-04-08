QUANTAXIS-Protocol
标准化协议QAS/未来协议QAF

------

- 当前版本:0.0.5
- 协议最后修改日期:2017-04-09
- 项目版本:QUANTAXIS 0.3.8-dev-RC(ARP)

<!-- TOC -->

- [QAS-00x Intro  简介](#qas-00x-intro--简介)
    - [QAS-001 About](#qas-001-about)
        - [QAS-001-1 关于QUANTAXIS](#qas-001-1-关于quantaxis)
        - [QAS-001-2 关于QUANTAXIS-Standard-Protocol](#qas-001-2-关于quantaxis-standard-protocol)
        - [QAS-001-3 关于QUANTAXIS-Future-Protocol](#qas-001-3-关于quantaxis-future-protocol)
    - [QAS-002 Module 模块](#qas-002-module-模块)
        - [QAS-002-1 Basical Module 基础模块](#qas-002-1-basical-module-基础模块)
            - [QAS-002-1-1 数据获取类 QAFetch](#qas-002-1-1-数据获取类-qafetch)
            - [QAS-002-1-2 数据存储/更新类 QASU](#qas-002-1-2-数据存储更新类-qasu)
            - [QAS-002-1-3 市场机制类 QAMarket](#qas-002-1-3-市场机制类-qamarket)
            - [QAS-002-1-4 回测类 QABacktest](#qas-002-1-4-回测类-qabacktest)
            - [QAS-002-1-5 账户/风险/组合管理类 QAARP](#qas-002-1-5-账户风险组合管理类-qaarp)
            - [QAS-002-1-6 工具类 QAUtil](#qas-002-1-6-工具类-qautil)
        - [QAS-002-2 Extension Module 扩展模块](#qas-002-2-extension-module-扩展模块)
            - [QAS-002-2-1 爬虫类 QASpider](#qas-002-2-1-爬虫类-qaspider)
            - [QAS-002-2-2 信号/事件驱动类 QASignal](#qas-002-2-2-信号事件驱动类-qasignal)
            - [QAS-002-2-3 任务机制/异步类 QATasks](#qas-002-2-3-任务机制异步类-qatasks)
            - [QAS-002-2-4 命令行扩展类 QACmd](#qas-002-2-4-命令行扩展类-qacmd)
        - [QAS-002-3 Mod 插件模块](#qas-002-3-mod-插件模块)
            - [QAS-002-3-1 QUANTAXIS-Webkit 插件](#qas-002-3-1-quantaxis-webkit-插件)
            - [QAS-002-3-2 QUANTAXIS-OpenCenter 插件](#qas-002-3-2-quantaxis-opencenter-插件)
    - [QAS-003 Criterion 规范](#qas-003-criterion-规范)
        - [QAS-003-1 模块命名方式](#qas-003-1-模块命名方式)
        - [QAS-003-2 函数命名方式](#qas-003-2-函数命名方式)
        - [QAS-003-3 数据库命名方式](#qas-003-3-数据库命名方式)
        - [QAS-003-4 RESTful 通信命名方式](#qas-003-4-restful-通信命名方式)
- [QAS-10x QAFetch 数据获取类](#qas-10x-qafetch-数据获取类)
- [QAS-20x QASU(save/update)数据存储/更新类](#qas-20x-qasusaveupdate数据存储更新类)
- [QAS-30x QAMarket 市场机制类](#qas-30x-qamarket-市场机制类)
- [QAS-40x QABacktest 回测类](#qas-40x-qabacktest-回测类)
- [QAS-50x QAARP(account/risk/portfolio)账户/风险/组合管理类](#qas-50x-qaarpaccountriskportfolio账户风险组合管理类)
- [QAS-60x QAUtil 工具类](#qas-60x-qautil-工具类)
- [QAS-70x QASpider 爬虫类](#qas-70x-qaspider-爬虫类)
- [QAS-80x QASignal 信号/事件驱动类](#qas-80x-qasignal-信号事件驱动类)
- [QAS-90x QATasks 任务机制/异步类](#qas-90x-qatasks-任务机制异步类)
- [QAS-100x QACmd 命令行扩展类](#qas-100x-qacmd-命令行扩展类)

<!-- /TOC -->


# QAS-00x Intro  简介
## QAS-001 About 
### QAS-001-1 关于QUANTAXIS
QUANTAXIS量化金融策略框架,是一个面向中小型策略团队的量化分析解决方案. 我们通过高度解耦的模块化以及标准化协议,可以快速的实现面向场景的定制化解决方案.QUANTAXIS是一个渐进式的开放式框架,你可以根据自己的需要,引入自己的数据,分析方案,可视化过程等,也可以通过RESTful接口,快速实现多人局域网/广域网内的协作.


### QAS-001-2 关于QUANTAXIS-Standard-Protocol
QUANTAXIS-Standard-Protocol(下称QAS)是为了规范化和标准化QUANTAXIS的数据获取,数据存储,模拟市场交易,以及标准化输出而建立的协议.通过遵守QAS协议,你可以快速的实现定制化需求,当然,你也可以在QAS的基础上增加自己的团队标准.

### QAS-001-3 关于QUANTAXIS-Future-Protocol
QUANTAXIS-Future-Protocol(下称QAF)是一些目前尚未实现或未添加的功能/想法,通过issue提交和pull request,你可以参与到QAF的定制与完善中来.

## QAS-002 Module 模块
QUANTAXIS是一个渐进式框架,所以会有基础模块和扩展模块之分
### QAS-002-1 Basical Module 基础模块
#### QAS-002-1-1 数据获取类 QAFetch
#### QAS-002-1-2 数据存储/更新类 QASU
#### QAS-002-1-3 市场机制类 QAMarket
#### QAS-002-1-4 回测类 QABacktest
#### QAS-002-1-5 账户/风险/组合管理类 QAARP
#### QAS-002-1-6 工具类 QAUtil
### QAS-002-2 Extension Module 扩展模块
#### QAS-002-2-1 爬虫类 QASpider
#### QAS-002-2-2 信号/事件驱动类 QASignal
#### QAS-002-2-3 任务机制/异步类 QATasks
#### QAS-002-2-4 命令行扩展类 QACmd
### QAS-002-3 Mod 插件模块
#### QAS-002-3-1 QUANTAXIS-Webkit 插件
#### QAS-002-3-2 QUANTAXIS-OpenCenter 插件

## QAS-003 Criterion 规范
### QAS-003-1 模块命名方式
### QAS-003-2 函数命名方式
### QAS-003-3 数据库命名方式
### QAS-003-4 RESTful 通信命名方式

# QAS-10x QAFetch 数据获取类
# QAS-20x QASU(save/update)数据存储/更新类 
# QAS-30x QAMarket 市场机制类 
# QAS-40x QABacktest 回测类
# QAS-50x QAARP(account/risk/portfolio)账户/风险/组合管理类
# QAS-60x QAUtil 工具类
# QAS-70x QASpider 爬虫类
# QAS-80x QASignal 信号/事件驱动类
# QAS-90x QATasks 任务机制/异步类
# QAS-100x QACmd 命令行扩展类