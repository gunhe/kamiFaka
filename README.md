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





### 3. 开发环境【如需修改或自定义，可查看该文档】

开发环境：[开发环境安装教程(自定义修改样式等等)](开发环境安装教程.md)


开源版访客页面：
![](https://cdn.jsdelivr.net/gh/Baiyuetribe/yyycode@dev/img/20/yyycode_comPc端演示.gif)
开源版管理员界面：
![](https://cdn.jsdelivr.net/gh/Baiyuetribe/yyycode@dev/img/20/yyycode_comPc后台端演示.gif)

## 🌱Github

项目已开通专属社区,主要集中开发者计划、BUG反馈、新功能建议等，欢迎积极参与讨论，[点此进入](https://github.com/gunhe/kamiFaka) 

## 🍳项目依赖
- 前端UI：Stisla --> https://github.com/stisla/stisla
- 前端交互程序：vue3.0 --> https://github.com/vuejs/vue-next
- 后端：Flask --> https://github.com/pallets/flask
- 管理员接口：Flask-JWT --> https://flask-jwt-extended.readthedocs.io/en/stable/

## 🍀部署方法：
```bash
# python  --version
# Python 3.8.12
# 卸载命令
docker rm -f kmfaka && docker rmi -f baiyuetribe/kamifaka:latest
# 构建命令
docker build  -t kmfaka-v001 .
# 安装命令
docker run --name kmfaka -itd --restart=always -p 8006:8000  kmfaka-v001:latest

# 后台地址 /admin
# 默认管理员 admin@qq.com 
# 默认密码 123456
```



## License

本程序使用MIT协议，您可以免费使用，复制或修改软件，但是请保留底部作者信息和License许可声明。
