# 求职简历

## 基本信息

* 姓名：吴龙怀     学历：全日制统招本科    工作经验：4年            微信/QQ：1053216036
* 年龄：26        手机：17520459207     邮箱：1053216036@qq.com   职位意向：Java后台开发工程师

## 教育经历

* 2011~2015      福建武夷学院         计算机科学与技术专业

## 工作经历

* 2017.6 ~至今         深圳市盈通供应链金融服务有限公司                   Java开发工程师
* 2016.6 ~2017.6      顺丰科技-企业内部系统研发中心-财务系统             Java开发工程师
* 2015.6 ~2016.6      厦门雅马哈信息系统-国内系统研发部                  Java开发工程师

## 技能清单

* 后端：Java基础，集合框架，多线程，JDBC，异常，流等
* 框架：Spring，SpringBoot，Mybatis，Shiro，Dubbo，Zookeeper
* 分布式：分布式缓存（Redis）、注册中心(Zookeeper)、消息队列(Kafka)、微服务架构、分布式事务、分布式调度、
* 数据库：Mysql（熟练），主从
* 测试：单元测试(熟练)，PostMan(熟练)，Jmeter（熟悉），Loadrunner（熟悉）
* 前端：Html(熟悉) CSS(熟悉) JavaScript(熟练) React + Redux(熟练) AntdPro(熟练)
* 运维：服务器(熟悉), Shell(熟悉), Docker(熟悉)，Nginx（负载均衡，反向代理），高可用（集群，主从，哨兵），定时任务备份，短信监控，证书
* 工具：Git(熟练)，Jenkins(熟练)，Maven(熟练)，PowerDesigner(熟练)，自动化构建/部署，版本代码质量管理

## 自我评价

常年从事企业级项目开发，熟悉财务、供应链行业、工厂的业务需求。不爱重复劳动，在项目开发过程中编写前端界面通用组件，模块化拆分复用模块，抽取主逻辑代码，编写代码生成器工具生成基本代码完成日常开发。能够接受突击的意外任务：曾经配合完成性能测试、运维生产环境搭建、自动化构建部署、在线客服的开发。喜欢新技术对微服务架构，容器化相关内容很感兴趣，针对其中的问题点会进行解决方案的构想和具体项目的实施。熟悉项目的需求研发上线运营的全流程，完整参与了盈通供应链金融服务有限公司的前后端分离微服务框架的选型和架构搭建和项目落地。

## 项目经验

### 一、[励响产业互联网平台](https://www.lx-device.com)

* 项目介绍

  励响设备运行保障平台是一个对制药企业、设备供应商和工程师进行资源整合和线上协同的供应链互联网平台，项目使用公司产品为基础根据励响网的业务结构进行设计和开发。针对医疗设备维修行业的上游药厂，下游供应商，工程师服务，配置了保障通（药企采购流程），技术通（工程师维修流程）的服务产品引入线上。

* 技术介绍

  react、antdpro、Springboot、Mybatis、zk/dubbo、redis、kafka、shiro、mysql、

* 我的职责

1. 代码生成器开发（设计和开发）：针对单表，主从类型表的基本界面进行前端组件抽象，前端代码功能配置化，后端代码进行抽象类以及组件整合，一套模板代码编写。在这个基础上编写代码生成器工具，加快了简单功能的代码编写工作量，提高交付效率。
2. 服务产品协同模块（设计和开发）：服务产品协同对平台中各个业务环节功能的执行顺序和数据依赖进行配置化的管理，通过配置化功能流程+代码扩展开发实现不同业务场景的需求。模块包含服务功能管理、服务产品管理（功能流程）、功能协同依赖、协同代办工作台、协同报表。
3. 询价、报价、订单、协议等基本业务功能前后端代码的开发。
4. 对客户进行敏捷开发的培训，定义代码管理流程上和上线测试发布流程，使用gogs+jenkins实现持续集成和交付，快速对软件进行迭代开发。
5. 生产环境的搭建，使用docker进行微服务部署，在架构方面实现了前端入口和后端入口的负载均衡和高可用，对于中间件redis、kafka、zookeeper、mysql进行高可用部署。完成https证书的请求加密。

### 二、盈通项目基础框架平台搭建

* 项目介绍

  基本框架的模块搭建，账户权限模块、通用数据权限配置、分布式事务、分布式调度，分布式会话，基础框架以及项目代码结构的搭建。

* 技术介绍

  dubbo、zookeeper、redis、kafka、springboot、shiro、react、antdpro、mysql

* 我的职责

1. 功能权限模块（设计和开发）：基于用户角色菜单权限模型，将系统的功能权限进行配置化管理，作为基础模块，通过Shiro管理精确到请求的后端权限验证，以及身份认证，并且将权限信息传递到前端界面实现前端的页面控制，用redis存储分布式会话，菜单权限使用缓存读取提高效率。
2. 数据权限模块（设计和开发）：设计人员维度关系，功能数据权限配置关系，将所有的系统功能添加一层可以配置的数据权限切面模块，实现按照人员 + 维度 + 功能的独立数据查询数据权限过滤，并且在新增和修改的时候也能够启用匹配校验，将权限校验精确到数据级别。
3. 鹰眼监控模块（设计和开发）：为了监控所有请求对应的异常情况，从业务起始步骤生成鹰眼Id，通过Dubbo的上下文透传到各个服务中，监控消息日志往kafka进行发送，统一进行异常的监控，生成请求的全链路调用堆栈。后端提示国际化实现类似。
4. 基础运维平台套件的架构和使用（设计和搭建）：使用Gogs+Jenkins+Maven进行代码审查以及持续构建，进行模块服务组装化的模块拆分，容器化部署服务，前后端实例及中间件都实现多机器高可用负载均衡的部署。

### 三、顺丰财务共享作业平台

* 项目介绍

  该项目是为了推动顺丰武汉财务共享中心信息化建设的平台，把原有的手动分单，预警监控以及数据统计分析工作搬到线上，并整合现有的外围填单系统各自的业务审批工作，实现财务审批统一入口，统一管理，提高共享中心整体时效和客户满意度；

* 技术介绍
  
  EasyUI、SSM、Java、Mysql、定时任务、定时调度、任务锁

* 我的职责

1. 智能分单平台开发:参与分单整体逻辑设计，数据库设计，完成任务模型配置，单据生成任务功能开发。
2. 实现单据接收接口以及审批流转接口，审批接口分别在不同系统中，互相认证来保证审核人身份权限。
3. 编写集群环境定时调度代码，保证在集群环境下分单任务的的定时执行使用分布式数据库锁的标记来控制。避免出现数据错乱问题，集群机器之间互斥但互不影响。

### 四、顺丰财务非集成线下表单系统

* 项目介绍
  搭建非集成线下表单系统把之前的线下表单的业务痛点（不同业务填写数据，业务流转，凭证接口数据有很大差异）使用动态配置的方式实现线下表单线上处理，接入EIS完成影像管理，接入ECP完成动态业务审批，调用智能分单平台完成财务审批，调用SAP完成固化凭证生成

* 技术介绍
  
  EasyUI、SSM、Java、Mysql、Jetty、单点登录、集群部署应用

* 我的职责

1. 集成线下表单系统：完成系统数据库设计和流程设计，完成前端动态明细区展示，表单整体流转实现。
2. 编写通用抽象类，实现不同单据类型对应审批接口的复杂数据准备，方便进行审批单据的添加和代码的扩展。
3. 编写xml格式数据文件解析，接受从SAP和ESB总线系统中传递的文件信息，使用多线程技术进行批量主数据导入。
4. 设计sap凭证生成依赖数据拼装的配置表，通过对表单配置不同的数据的引用依赖，以及公式计算，最后将变化部分数据和计算数据进行拆分，完成sap接口针对不同单据的复杂数据的拼装调用逻辑。
5. 对接各个业务系统，完成对应相关接口的业务和功能逻辑的开发

## 感谢您花时间阅读我的简历，期待能有机会和您共事
