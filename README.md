<p align="center">
  <a href="https://github.com/Baiyuetribe/kamiFaka">
    <img src="https://cdn.jsdelivr.net/gh/Baiyuetribe/baiyue_onekey@master/logo.png" alt="baiyue logo" width="90" height="90">
  </a>
</p>

<h1 align="center">佰阅发卡</h1>

<p align="center">
  基于VUE3.0+FLASK构建的全新卡密发卡系统
    <br>
    <img alt="GitHub Workflow Status (branch)" src="https://img.shields.io/github/workflow/status/Baiyuetribe/kamiFaka/%E8%87%AA%E5%8A%A8%E5%8C%96%E6%9E%84%E5%BB%BADocker%E9%95%9C%E5%83%8F/master?label=Docker&style=for-the-badge">
    <img alt="Docker Image Size (latest semver)" src="https://img.shields.io/docker/image-size/baiyuetribe/kamifaka?style=for-the-badge">
    <img alt="Docker Pulls" src="https://img.shields.io/docker/pulls/baiyuetribe/kamifaka?style=for-the-badge">
    <img alt="GitHub issues" src="https://img.shields.io/github/issues-raw/baiyuetribe/kamifaka?style=for-the-badge">

  <br>
  <a href="https://github.com/Baiyuetribe/kamiFaka/discussions">反馈 bug</a>
  ·
  <a href="https://kmfaka.baklib-free.com">教程 文档</a>
  ·
  <a href="https://www.bilibili.com/video/BV1Ra4y1p7QS">Vlog</a>
</p>

## 🎄开源版v1.8演示地址
海外演示1： http://107.148.243.178:8000

国内演示2： http://103.40.247.22:8000    [【该机器由茶猫云赞助,2天无理由退款+新购9折优惠】](https://www.chamaoyun.com/?u=D50390)             

后台地址`/admin`,默认管理员`admin@qq.com 123456`
## 🧰专业版v2.0演示地址
前台地址：http://119.29.25.39:3232/

后台地址：http://119.29.25.39:3232/admin

科技站： https://tech.baiyue.one

> 如果开源版不能满足你，可以尝试专业版，时隔一年多用新技术全部重写的一套专业自动售货系统。

## 💒适用场景：
适用于各种电商、优惠卷、论坛邀请码、充值卡、激活码、注册码、腾讯爱奇艺积分CDK等，支持手工和全自动发货，还有类似1688的分层批发模式。


## 🍭功能特色：

- Stisla UI：web界面很漂亮
- 前端使用VUE3.0,毫秒级响应
- 已集成支付宝当面付、微信官方、Payjs、虎皮椒、YunGouOS、易支付、Mugglepay、V免签等十几种支付接口
- 普通用户支持邮箱、短信接收消息
- 管理员支持邮箱、短信、TG、微信、QQ通知
- 支持2~4层批发模式
- 长卡密可导出为txt文本
- 多种主题模式【列表、卡片、宫格】
- 支持自定义背景、logo、联系方式等
- 支持热备份，可一键云端备份、一键导出备份文件到本地
- 数据库可分离，兼容Mysql、PostgreSQL和Sqlite
- 支持移动端唤醒支付宝
- JWT认证
- Limter保障服务器访问频率和次数
- 访客与管理员页面分离，可独立定制

## 🍀部署方法：

### 1. 正式环境【线上部署】
- [如何使用宝塔面板Docker管理器一键部署佰阅发卡](https://baiyue.one/archives/1703.html)

- [佰阅发卡KAMIFAKA：一款全新的基于VUE3.0+FLASK的卡密发卡系统](https://baiyue.one/archives/1700.html)

- [视频安装教程：【从0开始一步步使用宝塔Docker管理器搭建佰阅发卡v1.3版【2020】](https://www.bilibili.com/video/BV1Ra4y1p7QS) 

Github本地查看：[1.【宝塔+SQlite】](正式环境搭建教程.md#方法1宝塔nginxdocker数据库为sqlite)｜[2.【宝塔+Mysql】](正式环境搭建教程.md#方法2宝塔nginxdocker数据库为宝塔mysql)｜[3.【Heroku】](正式环境搭建教程.md#方法3heroku-无服务器部署)

### 2. 线上快速体验
Heroku 一键部署：[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://dashboard.heroku.com/new?template=https%3A%2F%2Fgithub.com%2FBaiyuetribe%2FkamiFaka)

个人服务器快速安装：
```bash
# 安装命令
docker run --name kmfaka -itd -p 8000:8000 baiyuetribe/kamifaka:latest
```
```bash
# 卸载命令
docker rm -f kmfaka && docker rmi -f baiyuetribe/kamifaka:latest
```

### 3. 开发环境【如需修改或自定义，可查看该文档】

开发环境：[开发环境安装教程(自定义修改样式等等)](开发环境安装教程.md)


开源版访客页面：
![](https://cdn.jsdelivr.net/gh/Baiyuetribe/yyycode@dev/img/20/yyycode_comPc端演示.gif)
开源版管理员界面：
![](https://cdn.jsdelivr.net/gh/Baiyuetribe/yyycode@dev/img/20/yyycode_comPc后台端演示.gif)

## 🌱Github社区讨论

项目已开通专属社区,主要集中开发者计划、BUG反馈、新功能建议等，欢迎积极参与讨论，[点此进入](https://github.com/Baiyuetribe/kamiFaka/discussions) 

## 🍳项目依赖
- 前端UI：Stisla --> https://github.com/stisla/stisla
- 前端交互程序：vue3.0 --> https://github.com/vuejs/vue-next
- 后端：Flask --> https://github.com/pallets/flask
- 管理员接口：Flask-JWT --> https://flask-jwt-extended.readthedocs.io/en/stable/

项目交流QQ群：853791822

- 官方帮助文档：[https://kmfaka.baklib-free.com](https://kmfaka.baklib-free.com)
- 专业版帮助文档： [http://119.29.25.39:3200/byfaka/](http://119.29.25.39:3200/byfaka)
- 专业版开发背景介绍： https://baiyue.one/archives/1785.html
## 🌱案例展示

<p align="center">
    <br>

  <br>
  <a href="https://faka.ludeqi.com/" target="_blank"><img alt="demo" src="https://faka.ludeqi.com/images/logo.png"></a>
  <a href="http://400718.com/" target="_blank"><img alt="小郎发卡" src="http://400718.com/images/logo.png"></a>
  
</p>


## 🍰其他自研项目推荐
- [人工智能桌面APP](https://github.com/Baiyuetribe/paper2gui)
- [Glink跨平台短视频去水印解析](https://baiyue.one/archives/1736.html)
- [阿里云盘列表alist_fiber](https://baiyue.one/archives/1726.html)

## License

本程序使用MIT协议，您可以免费使用，复制或修改软件，但是请保留底部作者信息和License许可声明。


## 环境依赖
```bash
# python  --version
# Python 3.8.12
```