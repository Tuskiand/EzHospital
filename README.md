# Hospital-Registration-Platform

基于Spring Boot和微信小程序的医院预约挂号平台，包含三端应用: 
- 后端 API 服务
- Web 管理系统
- 微信小程序

## 系统架构

### 后端技术栈
- Spring Boot
- MyBatis
- MySQL
- Redis 
- Swagger-UI
- JWT

### Web 前端技术栈
- Vue.js
- Element UI
- Axios

### 小程序技术栈
- uni-app
- WeUI

## 主要功能

### 小程序端
- 用户注册/登录
- 预约挂号
- 就诊卡管理
- 就诊记录查询
- 个人中心

### Web 管理端
- 医院信息管理
- 科室管理
- 医生排班管理
- 预约信息管理
- 用户管理

## 环境准备

### 所需环境
- JDK 1.8+
- MySQL 5.7+
- Redis 3.0+
- Node.js 12+
- npm 6+
- 微信开发者工具

## 部署步骤

### 1. 后端部署
1. 确保基础服务已启动:
   - MySQL(必需)
   - Redis(可选)
   - 短信服务(可选)
   - 对象存储服务(可选)

2. 使用 IDEA 运行:
```bash
运行 HospitalApplication.java
```

3. 访问接口文档:
```
URL: http://localhost:6789/hospital/doc.html
账号: hospital
密码: hospital
```

### 2. Web 管理系统部署
1. 进入项目目录:
```bash
cd hospital-web-master
```

2. 安装依赖:
```bash
npm install
```

3. 运行开发服务器:
```bash
npm run dev
```

4. 访问系统:
```
账号: admin
密码: admin
```

### 3. 小程序部署
1. 打开Hbuilder X 打开目录：hospital-wxapp-master
2. 发行-小程序 微信
3. 打开微信开发者工具 导入：hospital\hospital-wxapp-master\unpackage\dist\build\mp-weixin
4. 点击编译运行

注: 默认手机验证码为 123456

## 注意事项

1. 用户注册要求:
   - 手机号需符合标准格式
   - 身份证号需符合标准格式
   - 密码必须为字母+数字的组合

2. 权限模块说明:
   - 用户权限模块尚未开发完成
   - 本项目暂不涉及该功能

3. 手机真机调试:
   - 需要电脑和手机连接同一WiFi
   - 配置HTTPS抓包
   - 使用开发者工具生成预览二维码
   - 微信扫码即可在手机上预览


## 数据库
- 数据库文件位置: hospital\hospital-master\src\main\resources\hospital.sql
- 需要提前创建数据库并导入该SQL文件

## 贡献
欢迎提交Issues和Pull Requests

## License
MIT License