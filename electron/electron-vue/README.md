# Electron + Vue 3 + TypeScript + Vite

这个模板应该可以帮助您开始使用Vite中的Vue 3和TypeScript进行Electron桌面应用开发。
该模板使用Vue 3 `<script setup>`,[script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup)
SFC，请查看脚本设置文档以了解更多信息。

## 推荐的IDE设置

- [VS Code](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar)

## 运行

```bash
yarn
yarn dev
```

or
```bash
npm install
npm run dev
```

# 打包过程中可能遇到的问题

## 1.打包时下载electron-v.xxxx.zip文件失败

解决办法：直接在淘宝的文件库下载对应版本和打包平台的文件，下载完成后放在C:
\Users\Administrator\AppData\Local\electron\Cache这个目录下

## 2.打包时下载winCodeSign-v.xxx.7z文件失败

下载地址：https://github.com/electron-userland/electron-builder-binaries/releases/download/winCodeSign-2.5.0/winCodeSign-2.5.0.7z
下载完解压放到C:\Users\Administrator\AppData\Local\electron-builder\Cache\winCodeSign目录下

## 3.打包时下载nsis-v.xxx.7z文件失败

下载地址：https://github.com/electron-userland/electron-builder-binaries/releases/download/nsis-3.0.4.1/nsis-3.0.4.1.7z
下载完解压放到C:\Users\Administrator\AppData\Local\electron-builder\Cache\nsis

## 4.打包时下载nsis-resources-v.xxx.7z文件失败

下载地址：https://github.com/electron-userland/electron-builder-binaries/releases/download/nsis-resources-3.4.1/nsis-resources-3.4.1.7z
下载完解压放到C:\Users\Administrator\AppData\Local\electron-builder\Cache\nsis\nsis-resources-3.4.1

> 第2、3、4步下载的文件如果需要其他版本，直接修改链接中的版本号即可

# 更新依赖

```bash
npm install npm-check-updates --global
ncu -u
```

or

```bash
yarn upgrade-interactive --latest
```

检测到需要更新的包后，空格键可以选择或取消单个需要更新的包，A键可以切换所有需要更新的依赖包，最后回车即可更新。