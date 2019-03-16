# 一键部署 v2ray 到 heroku  
[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)
- - -
- - -
0.Fork自https://github.com/wpyok500/Heroku-v2ray-1。最高支持v2ray 3.46

1.部署时配置 v2ray core 的版本、Vmess协议的UUID、AlterId、Path和连接缓存。

2.v2ray服务端部署后,v2ray端口为443

3.如果输入AppName变量，则自动生成订阅地址和二维码，通过配置V2_QR_Path变量修改地址
二维码地址：https://test.herokuapp.com/1234/v2.png
订阅地址：https://test.herokuapp.com/1234 (test改成自己的app名称，如果更改了V2_QR_Path，同时也要将对应的1234改成修改后的)

4.服务端部署后，点 open app ，能正常显示网页，地址补上path后访问显示 Bad Request，表示部署成功。

5.更新 v2ray 版本，访问 https://dashboard.heroku.com/apps 选择部署好v2ray的app，如果VER变量为 latest。直接选择More --> Restart all dynos, 程序自动重启，可通过view Logs确认进度。（更新指定版本： Settings --> Reveal Config Varsapp -->VER，修改成需要的版本号，例如 3.21）

# 参考 
https://github.com/v2ray/v2ray-core

https://github.com/wangyi2005/v2ray-heroku

https://github.com/1715173329/v2ray-heroku-undone

https://github.com/ki8852/v2ray-heroku-undone
