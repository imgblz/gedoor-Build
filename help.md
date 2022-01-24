## 在线编译legado阅读3.0(不用本地编译了)

使用了github actions自动构建

可以随时基于最新代码编译你自己的阅读3.0,和已有阅读3.0共存

fork到你自己的仓库,或者在本仓库右上角点一下Star就会自动开始编译

已经Star的点Unstar,再点Star会再次开始编译

大概十多分钟就会编译好

编译好的apk自动打包为legado.apk.zip,去你自己的Actions里找

默认自动清空 18PlusList.txt

安装失败(-102)和与已安装应用签名不同问题已解决

多个APP共存问题通过修改applicationIdSuffix='.releaseA',不用卸载重装了

增加一系列任务脚本,比如action_app_custom.sh用来个性化定制app

本项目现在可以对任意android项目进行自动化构建了,只需要更新一下脚本就可以了

支持阅读2.0 3.0

修改action_setenv.sh脚本里的坏境变量APP_NAME,APP_GIT_URL

APP_NAME='MyBookshelf'

APP_GIT_URL='https://github.com/gedoor/MyBookshelf.git'
