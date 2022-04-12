# transmission-web-control-Synology
Transmission WebUI管理面板安装脚本 群晖DiskStation优化版 
Transmission WebUI Installation Shell Script for Synology DiskStation.

## 介绍 / Introduction
源项目[ronggang/transmission-web-control](https://github.com/ronggang/transmission-web-control)，本项目是在其脚本原有的基础上作些许修改。

由于群晖DSM 6.2.3-25426从源安装的wget-ssl版本老旧，不支持*TLS1.2*协议，因此将脚本内的**wget**替换成**curl**方便使用。

且因源项目中，面向中国大陆用户的[Gitee仓库版本](https://gitee.com/culturist/transmission-web-control)因为长时间未更新，项目与ronggang/transmission-web-control仓库差了不少commit，因此CDN版脚本采用反向代理镜像站方法获取项目源码。

## 使用方法 / How To Use
中文菜单：
```shell
curl -O --insecure https://raw.githubusercontent.com/0xCP/transmission-web-control-Synology/main/DiskStation6-install-tr-control-Chinese.sh
bash DiskStation6-install-tr-control-Chinese.sh
```
中文菜单(中国大陆CDN优化)：
```shell
curl -O --insecure http://cdn.jsdelivr.net/gh/0xCP/transmission-web-control-Synology@main/DiskStation6-install-tr-control-CDN.sh
bash DiskStation6-install-tr-control-CDN.sh
```
英文菜单 / English：
```shell
curl -O --insecure https://raw.githubusercontent.com/0xCP/transmission-web-control-Synology/main/DiskStation6-install-tr-control.sh
bash DiskStation6-install-tr-control.sh
```
