# 鹿途后台管理系统
## 准备工作
* 安装 angular 环境
* 安装 ng-zorro 依赖
## 即开即用
[鹿途系统基础框架](https://github.com/ZhouRenYou/ng-project)：这是鹿途管理系统一个干净基础的框架，即开即用，如果你觉得方便，就给我一个小星星吧 😊
## 文档中心

[博客园——鹿途](https://www.cnblogs.com/zry2510/category/1096539.html)

[基于qrious生成二维码](https://www.zhourenyou.com/2019/04/26/qrious/)

[实现鹿途系统在线演示功能的方法](https://www.zhourenyou.com/2019/03/25/ng-page/#more)

#### 项目操作表格功能时，数据变动请关注console

[Live](https://zhourenyou.github.io/web-deerway/) 


## 项目说明

## 开始

### 创建项目
`
ng new ng-deerway --style less
`

`
cd ng-deerway
`
### 初始化配置
`
ng add ng-zorro-antd
`
### 安装组件   
`
npm install ng-zorro-antd --save
`
## 运行

`ng s -c [environment] --port [port]`


## 快捷指令

快速生成模块

`
ng g m [保存位置]/modelName
`

快速生成组件

`
ng g c [保存位置]/componentName
`

快速生产服务

`
ng g s [保存位置]/serviceName
`

快速生产管道

`
ng g pipe [保存位置]/pipeName
`


## 项目结构

> * core ng-zorro组件二次封装 通用服务、管道以及通用验证
> * layout   通用模版
> * routes   项目主体内容
> * shared   导入导出项目公用的引用
> * styles   通用样式
> * assets   静态资源（图片与图标）

## ng-zorro组件二次封装(app/shared/meta)
> * 基础表格组件 dw-table
> * 通用时间组件 dw-date-picker
> * 通用搜索组件 dw-search
> * 信息模态框 dw-info-model
> * 分页组件 dw-pagination
> * 动态表格组件 dw-table-dynamic

### 用户认证

[@delon/auth](https://ng-alain.com/auth/getting-started)

## 第三方资源

图标：[iconfont](http://iconfont.cn)

地图：[angular-baidu-maps](https://github.com/cipchk/angular-baidu-maps)

图表：[echarts](http://echarts.baidu.com/index.html)

## 部署

#### 1、打包
`
ng build --prod
`
#### 2、配置WEB服务服务器
[nginx](http://www.nginx.cn/doc/)

#### 3、推送资源

`
scp -r  打包后文件路径 root@服务器IP地址：/root/www
`
#### 4、域名解析，发布完成


