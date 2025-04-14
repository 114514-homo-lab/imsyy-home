README.md 原文可点击[这里](https://github.com/imsyy/home/blob/dev/README.md)查看。

[<img alt="Deployed with FTP Deploy Action" src="https://img.shields.io/badge/Deployed With-FTP DEPLOY ACTION-%3CCOLOR%3E?style=for-the-badge&color=0077b6">](https://github.com/SamKirkland/FTP-Deploy-Action)

# Home
此仓库由[imsyy](https://github.com/imsyy/home)改进而来。
由

# Changelog
增加了ftp部署站点 <br>
在 GitHub Actions 中新增使用 sed 命令更改高德 API 的功能，以保护高德 API 不被泄露。<br>
增加了企业名 <br>

# 说明
因 GitHub Actions 的镜像从 windows-latest 更改为 ubuntu-latest，因此`.env.example`自动更改`.env`已失效，因此直接套用原仓库将无法使用。

# How to Use
1. Fork 本仓库
2. 在 Settings => Actions secrets and variables => Actions => Repository secrets 中添加以下变量：
   - `ftp_server`：ftp服务器
   - `ftp_password`：ftp密码
   - `ftp_username`: ftp用户名
   - `AMAP_KEY`：高德地图 API Key
3. commit 任意一个 dev 分支下的一个文件，启动 Actions 编译。即可成功部署你的网站。
