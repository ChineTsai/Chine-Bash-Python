# Chine-Bash-Python 多用户管理脚本（基于官方mujson版本）
- [x] 稳定版V1.7.2：[![Build Status](https://travis-ci.org/Readour/AR-B-P-B.svg?branch=master)](https://travis-ci.org/Readour/AR-B-P-B)  [![Code Climate](https://codeclimate.com/github/Readour/AR-B-P-B/badges/gpa.svg)](https://codeclimate.com/github/Readour/AR-B-P-B)

- [x] 开发版V1.9.8：[![Build Status](https://travis-ci.org/Readour/AR-B-P-B.svg?branch=develop)](https://travis-ci.org/Readour/AR-B-P-B)

## 介绍 ##

涉密数据加密传输系统，有效对抗政府对互联网的网络审查，基于Shell脚本和Python语言编写，集成多用户管理、流量限制、加密更改等基本操作。

- 该版本将由本人开发和更新，同时保持所有代码完全开源！
- 请谨慎使用，使用期间出现任何问题概不负责！！！！
- 如果发现脚本bug，可以发issues，但不一定会去fix，多谢合作！

## 系统支持 ##
* Ubuntu 14
* Ubuntu 16
* Debian 7
* Debian 8
* CentOS 6
* CentOS 7

## 功能 ##
- 全自动无人值守安装，服务端部署只需一条命令
- 一键开启、关闭服务
- 添加、删除、修改用户端口、密码和连接数限制
- 支持傻瓜式用户添加
- 自由限制用户端口流量使用及端口网速
- 自动修改防火墙规则
- 自助修改加密方式、协议、混淆等参数
- 自动统计，方便查询每个用户端口的流量使用情况
- 自动安装Libsodium库以支持Chacha20等加密方式
- 支持用户二维码生成(有bug，仅开发版可用)
- 支持一键构建panel-V3-mod,前端后端自动对接，无需额外操作（仅开发版可用）
- 傻瓜式BBR、锐速、LotServer一键构建（有风险，仅开发版可用）
- 可自定义的服务器巡检，故障自动重启服务，确保链接稳定有效
- 可对配置进行备份、还原，迁移服务器只需在新服务器上还原配置，无需重复设置
- 支持IP黑名单功能，可通过端口查询，直接加入黑名单，禁止该IP访问服务器的所有服务
- 允许针对不同用户限制帐号有效期，到期自动删除帐号

实际操作界面:

![](https://github.com/zyh001/zyh001.github.com/raw/master/images/now1.png) ![](https://github.com/zyh001/zyh001.github.com/blob/master/images/now2.png)

正在开发界面：
![](https://github.com/zyh001/zyh001.github.com/blob/master/images/future.png)

## 脚本安全性声明 ##
**本脚本采用Shell和Python语言编写，所有代码完全开源。不存在所谓的后台或挖矿代码，不会对您的任何信息进行上传，并在各个方面充分考虑到数据安全性。关于二维码生成过程是通过pip安装[第三方软件包](https://github.com/lincolnloop/python-qrcode)，由第三方软件在服务器本地生成，生成的二维码链接也会自动销毁，不会上传任何信息。您的IP被封，或者您服务器出现不正常的负荷增高，与脚本本身没有任何关系，请您自行做好服务器安全维护工作，例如：不要使用弱密码、不要使用默认SSH端口，等等，防止被闲人爆破。**


## 安装&更新 ##
    wget -q -N --no-check-certificate https://raw.githubusercontent.com/FunctionClub/SSR-Bash-Python/master/install.sh && bash install.sh

## 系统自检 ##
    wget -q -N --no-check-certificate https://raw.githubusercontent.com/FunctionClub/SSR-Bash-Python/master/self-check.sh && bash self-check.sh

## 卸载 ##
    wget -q -N --no-check-certificate https://raw.githubusercontent.com/FunctionClub/SSR-Bash-Python/master/install.sh && bash install.sh uninstall

## 离线安装 ##
    #此方法可用于网络情况不好，导致缺少文件的情况.亦可下载该脚本，用于备份
    wget -q -N --no-check-certificate https://down.fdos.me/install.sh && bash install.sh
    
## 客户端下载 ##
常用平台：[Android](https://github.com/shadowsocksrr/shadowsocksr-latest-bin-backup/raw/master/Shadowsocksr-android-3.4.0.5.apk)、[MacOS](https://github.com/qinyuhang/ShadowsocksX-NG-R/releases/download/1.4.3-R8/ShadowsocksX-NG-R8.dmg)、[Windows](https://github.com/Readour/ShadowsocksR-Csharp/releases/download/4.7.0/ShadowsocksR-4.7.0-win.CONCISE.7z)、[Linux](https://github.com/shadowsocks/shadowsocks-qt5/releases/download/v2.9.0/Shadowsocks-Qt5-x86_64.AppImage)、[OpenWrt/LEDE](https://github.com/bettermanbao/openwrt-shadowsocksR-libev-full/releases)、[iOS](https://github.com/Readour/breakwa11.github.io/raw/master/download/Shadowrocket%202.1.14.ipa)

## In the End ##
<span style="font-size:18px;"><span style="color:#E53333;"></span></span><span style="font-size:16px;color:#E53333;">**中华人民共和国网络审查办法：**</span>根据《国务院关于授权国家互联网信息办公室负责互联网信息内容管理工作的通知》，自2014年8月26日起，国家互联网信息办公室（简称国家网信办，与中共中央网络安全和信息化领导小组办公室为一个机构两块牌子，牌子挂在国务院新闻办公室）负责中国大陆互联网信息内容管理工作，并负责监督管理执法。:sunny:
