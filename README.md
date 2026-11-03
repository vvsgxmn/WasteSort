# 基于SpringBoot+Vue的垃圾分类系统

![Spring Boot](https://img.shields.io/badge/-Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white) ![Vue3](https://img.shields.io/badge/-Vue3-grey?style=flat-square) ![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![MyBatis](https://img.shields.io/badge/-MyBatis-000000?style=flat-square&logo=mybatis&logoColor=white) 

## 项目介绍

本系统是一款面向社区居民与环卫监管场景的垃圾分类服务平台，针对分类标准记不住、可回收物预约上门不方便、积分兑换与违规投放缺少闭环、科普宣教和督导整改互相脱节等问题，把分类百科查询、预约回收、积分商城、知识挑战、志愿活动、违规上报，以及管理员驾驶舱整合到同一套前后端分离工程中。

系统采用 SpringBoot + Vue 架构，区分居民与系统管理员两类角色：居民查询投放标准、预约上门回收、用积分兑换商品并参与答题和志愿活动；管理员维护分类规范与垃圾条目、审核回收工单与兑换订单、处理违规督导整改并查看 ECharts 运营指标。回收工单从预约、接单到完成可追溯，违规上报进入整改台账，适合作为毕设、课设与智慧环卫学习参考。

## 主要功能模块

- **用户认证与角色分流**：居民注册登录、管理员统一登录，JWT 鉴权；登录后进入居民前台或监管中台，管理端路由与接口双重隔离
- **分类百科**：按可回收物、有害垃圾、厨余垃圾、其他垃圾查询条目与投放说明，支持关键词检索和详情浏览
- **预约回收**：居民填写品类、重量、地址与上门时间提交工单，在我的回收中跟踪待接单、进行中与已完成状态
- **积分商城**：完成分类与回收获得积分，兑换实物或权益；兑换订单可查询发货进度，积分流水可追溯
- **知识挑战**：按题库作答垃圾分类题目，答对累计积分，巩固投放标准
- **志愿活动与科普**：报名环保志愿活动，阅读政策资讯与分类科普文章
- **违规上报**：居民拍摄并上报混投、乱堆等现场，填写地点与说明，形成督导线索
- **运营驾驶舱**：回收量、工单、积分兑换与上报等 KPI，以及分类占比、趋势等 ECharts 图表
- **分类与知识库中台**：维护四大分类规范、垃圾条目图文、题库、科普文章与志愿活动
- **工单与积分监管**：审核回收预约、处理兑换发货、查询积分流水与用户账户
- **违规督导整改**：受理上报、派发整改并回写处理结果，形成上报到闭环的台账
- **论文与 UML 概览**：配套论文设计实现页拼图与 UML 图列表，便于答辩材料对照

## 技术架构

- **后端**：Spring Boot + MyBatis-Plus + JWT + Lombok
- **前端**：Vue 3 + TypeScript + Vue Router + Pinia + Element Plus + Vite + ECharts
- **数据库**：MySQL

<!-- screenshots-start -->
## 系统截图

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/wastesort/%E7%99%BB%E5%BD%95%E9%A1%B5%E9%9D%A2.png" alt="登录页面" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/wastesort/%E7%94%A8%E6%88%B7%E9%A6%96%E9%A1%B5.png" alt="用户首页" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/wastesort/%E5%88%86%E7%B1%BB%E7%99%BE%E7%A7%91.png" alt="分类百科" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/wastesort/%E7%A7%AF%E5%88%86%E5%95%86%E5%9F%8E.png" alt="积分商城" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/wastesort/%E8%BF%9D%E8%A7%84%E4%B8%8A%E6%8A%A5.png" alt="违规上报" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/wastesort/%E7%AE%A1%E7%90%86%E5%91%98%E9%A9%BE%E9%A9%B6%E8%88%B1.png" alt="管理员驾驶舱" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/wastesort/%E5%9E%83%E5%9C%BE%E7%9F%A5%E8%AF%86%E5%BA%93%E7%AE%A1%E7%90%86.png" alt="垃圾知识库管理" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/wastesort/%E8%BF%9D%E8%A7%84%E7%9D%A3%E5%AF%BC%E6%95%B4%E6%94%B9.png" alt="违规督导整改" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/wastesort/%E8%AE%BA%E6%96%87%E5%9B%BE1.png" alt="论文图1" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/wastesort/%E8%AE%BA%E6%96%87%E5%9B%BE2.png" alt="论文图2" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/wastesort/UML%E5%9B%BE%E5%88%97%E8%A1%A8.png" alt="UML图列表" width="600" />

<!-- screenshots-end -->

## 接毕业设计和论文

### 作者微信：vvsgxmn  (支持修改、 部署调试、 支持代做毕设)

### 接网站建设、小程序

### 选题+开题报告+任务书+程序定制+安装调试+论文+答辩ppt 都可以做

### 购买地址：[https://www.vvxx.love](https://www.vvxx.love)（vv毕设网）

### 支持 **一键生成 UML 图**：上传项目压缩包即可自动产出功能模块图、用例图、流程图、E-R 图、时序图等全套毕设图表。

### 提供 **免费配套软件下载 + 安装说明 + 部署教程**

![vv毕设网 - 一键画图](https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/uml-draw.png)

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/image-20260825133349317.png" alt="image-20260825133349317" />

⚠️ Bug添加微信**免费修复**，免费修复。其他平台的私信一律不管（微信方便发送文件）
