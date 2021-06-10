
QQ付费入群系统
===============
QQ付费入群系统 是基于 V发卡（ https://github.com/szvone/Vfkphp ）   
二次开发实现的一套自动入群程序，主要包含以下特色：

 + 完全开源
 + 对接v免签，实现配套免签约自动回调
 + 提供Nonebot2插件，支持24小时审核入群
 

> QQ付费入群系统仅供个人开发者调试测试和交流学习使用，请勿用于非法用途

> bug反馈请建立issues

> Mirai机器人插件-推荐（ https://github.com/LittleTurtle2333/pay_join_group_mirai ）

> Nonebot2机器人插件（ https://github.com/LittleTurtle2333/pay_join_group_nonebot2 ）

> V免签PHP服务端（ https://github.com/szvone/vmqphp ）

> V免签监控端（ https://github.com/szvone/vmqApk ）
## 前言

QQ付费入群系统为完全开源项目，开源项目意味着作者没有任何收入来源，仅凭个人空闲时间开发，点击上面的Star给一个星星，也是对我莫大的认同，感谢各位的支持。

## 安装
 + 推荐使用宝塔面板安装，以下教程为宝塔面板安装教程，其他环境请参考自行配置

    1、下载源代码,Clone or download->Download ZIP
    
    2、宝塔面板中新建网站，设置：
        
        + 网站目录->运行目录 设置为public并保存
        + 伪静态 设置为thinkphp并保存
        + 默认文档 设置将index.html放在第一行并保存
    
    3、打开网站目录 config/database.php ，设置好您的mysql账号密码。
    
    4、导入数据库文件（位于根目录）fk2.sql到您的数据库。
    
    5、设置宝塔计划任务，访问URL，执行周期为每1分钟，访问内容为：http://域名/closeOrder
    
    6、至此网站搭建完毕，请访问后自行修改配置信息！后台登录地址：http://域名/login.html ，默认后台账号和密码均为admin

    7、请在V免签中设置您的回调地址：
    
        同步回调：http://您的域名/payReturn
        异步回调：http://您的域名/payNotify

 > 升级说明：请您直接下载新版本覆盖旧版本即可！

## 调用

 + 请部署完成后访问后台，有详细的Api说明
 
## 注意

  + 本系统为对接v免签实现的一套QQ付费入群系统，所以请您在使用本套系统之前先部署v免签
  
  + QQ付费入群系统面向用户是个人开发者，如果您不懂如何开发网站，那么v免签不适合您的使用！
  
  + QQ付费入群系统是免费开源产品，所有程序均开放源代码，所以不会有收费计划，因此作者不可能教会每个人部署安装，请参考文档多百度谷歌，v免签使用具有一定的技术门槛，请见谅！

## 版权信息

QQ付费入群系统遵循 MIT License 开源协议发布，并提供免费使用，请勿用于非法用途。

## 感谢
> V发卡（ https://github.com/szvone/vfkphp ）

> V免签PHP服务端（ https://github.com/szvone/vmqphp ）

> V免签监控端（ https://github.com/szvone/vmqApk ）
