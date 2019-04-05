V2ray官方安装步骤
==================================
**安装<br>**
bash <(curl -L -s https://install.direct/go.sh)

[V2ray配置在线生成](https://intmainreturn0.com/v2ray-config-gen/)

V2Ray 程序
/usr/bin/v2ray/v2ray

V2Ray 工具
/usr/bin/v2ray/v2ctl

配置文件
/etc/v2ray/config.json

IP 数据文件
/usr/bin/v2ray/geoip.dat

域名数据文件
/usr/bin/v2ray/geosite.dat

重启v2ray
sudo systemctl restart v2ray

查看v2ray运行状态（active）
service v2ray status

安装GUI
-----------------------------------------
**1.安装Gnome包<br>**
yum groupinstall "GNOME Desktop" "Graphical Administration Tools"<br>

**2.更新系统的运行级别<br>**
ln -sf /lib/systemd/system/runlevel5.target /etc/systemd/system/default.target<br>

**3.重启机器,启动默认进入图形界面<br>**
reboot<br>

**PS:未进入，重新连接输入<br>**
startx

---------------------------------

v2ray(233版)一键安装步骤--此仓库版本
--------------------------------
**脚本说明<br>**
V2Ray 一键安装脚本

**搭建教程<br>**
[V2Ray搭建详细图文教程](https://github.com/233boy/v2ray/wiki/V2Ray%E6%90%AD%E5%BB%BA%E8%AF%A6%E7%BB%86%E5%9B%BE%E6%96%87%E6%95%99%E7%A8%8B)

**安装<br>**
wget -N --no-check-certificate https://raw.githubusercontent.com/fxuan2030/V2Ray/master/install.sh && chmod +x install.sh && bash install.sh


**快速管理<br>**
v2ray info 查看 V2Ray 配置信息<br>
v2ray config 修改 V2Ray 配置<br>
v2ray link 生成 V2Ray 配置文件链接<br>
v2ray infolink 生成 V2Ray 配置信息链接<br>
v2ray qr 生成 V2Ray 配置二维码链接<br>
v2ray ss 修改 Shadowsocks 配置<br>
v2ray ssinfo 查看 Shadowsocks 配置信息<br>
v2ray ssqr 生成 Shadowsocks 配置二维码链接<br>
v2ray status 查看 V2Ray 运行状态<br>
v2ray start 启动 V2Ray<br>
v2ray stop 停止 V2Ray<br>
v2ray restart 重启 V2Ray<br>
v2ray log 查看 V2Ray 运行日志<br>
v2ray update 更新 V2Ray<br>
v2ray update.sh 更新 V2Ray 管理脚本<br>
v2ray uninstall 卸载 V2Ray<br>

配置完成无法联网请关闭VPS防火墙<br>
<br>
查看防火墙状态<br>
firewall-cmd --state<br>
停止firewall<br>
systemctl stop firewalld.service<br>
禁止firewall开机启动<br>
systemctl disable firewalld.service <br>

