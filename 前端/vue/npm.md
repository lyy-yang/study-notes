2021/8/2

<h3 style='color:green'>
    npm相关命令：
</h3>

```
node -v
npm -v

npm install npm (-g)
全局安装，该命令在命令行上可以任意一个地方去使用，使得装的包在别的地方也能用

npm install jquery (-g)  默认安装最新版本
npm install bootstrap
dir查看目录下文件/目录结构
cls清屏
npm list (-g)  查看(全局)安装的包
npm list jquery  单独查看某一个包的版本号
npm install jquery@3.0.0  指定版本
npm update jquery  更新版本
npm uninstall jquery  卸载

(在package文件中的dependencies节点写入依赖，默认sava)
npm install jquery -save  运行时依赖
npm install babel-cli -save-dev  开发时依赖

```

装的是一个包，这个包可以生成一个命令，命令在任意地方都可以用，把包装到环境变量里面去

install可以缩写成i



<h3 style='color:green'>
    镜像的使用：
</h3>

```
使用镜像，下载npm会快一点

得到配置文件，查看这个包从哪个地方下载过来的
npm config get registry
或者
npm config get disturl

设置配置文件
npm config set registry http://registry.npm.taobao.org (--global全局设置镜像，在别的地方也是从这里下载)

使用nrm工具切换淘宝源
npx nrm use taobao

切回官方源
npx nrm use npm

设置默认npm下载地址
npm config set registry heep://registry.npmjs.org

重新命名，使用cnpm到淘宝下载，使用npm到外国网站下载
$npm install -g cnpm --registry=http://registry.npm.taobao.org
```



<h3 style='color:green'>
    package.json配置文件：
</h3>

```
生成配置文件：
npm init --yes
运行脚本e.g.
npm run test
```



版本前的^和~符号

^3.X.X     ~3.5.X