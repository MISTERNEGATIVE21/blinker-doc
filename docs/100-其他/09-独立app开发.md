# app开发（beta）

## App打包上架服务  

### 免费打包服务
仅面向专属设备可用数量1000个以上的开发者提供android Apk打包服务，每个开发者账号每月限1次。  

APP打包需要提供的资料：  
应用名：该App名称（中文或英文）  
包名：\<xxx\>.diandeng.tech  
App图标：<1024 x 1024  PNG格式>  
启动页图片：<2700 x 2700  PNG格式>（请图片中包含应用或企业名称）  
登录页logo：<不超过700 x 200 PNG格式>（务必背景透明）  

打包后的apk文件未签名，用户自行签名后，可发布到应用商店。  

#### android App签名方法
1.安装jdk
2.在jdk\bin下，运行如下命令生成密钥：
```bash
keytool -genkey -alias <name> -keyalg RSA -validity 10000 -keystore <name>.keystore
```
<name>为自定义的名称  
3.使用如下命令进行签名：
```bash
jarsigner -verbose -keystore <name>.keystore -signedjar <apkfilename>_signed.apk <apkfilename>.apk <name>.keystore  
```

如用户不想自行签名发布，可使用我们提供的发布服务：  

### Android打包签名上架服务  
收费标准：15000元/年（包含一年时间内对App的维护和更新）  
默认上架市场：腾讯应用宝  
上架其他市场收费：500元/次/个  
其他说明：
1. 上架应用需要提供软件著作权证书，所产生费用由开发者承担；  
2. 资料齐备后，首次上架通常3~7个工作日，具体时间由应用商店方面决定。  

### IOS打包上架服务  
需要提供的资料同android  
收费标准：15000元/年（包含一年时间内对App的维护和更新，不包含注册开发者账号产生的相关费用）  
其他说明：
1. 上架应用需要苹果开发者账号，所产生费用由开发者承担；  
2. 由于IOS版本发布审核上线流程严格，手续繁琐，所以版本发布通常会有滞后，具体时间由苹果公司方面决定。  

## 企业版  
企业版可使用现blinker app的所有功能，可定制，亦可二次开发。  
企业用户可联系：  
![](../img/099/dongbo.png)  

## 开源版本  
[历史版本](https://github.com/blinker-iot/blinker-app)  
项目基于cordova8、ionic5、angular8开发，可自行了解相关技术。  

## blinker-Customizer  
以嵌入web app的方式，开发独立的blinker设备页面。[了解更多](https://diandeng.tech/docs/009-专属设备开发/09-Customizer定制设备界面.md)  
