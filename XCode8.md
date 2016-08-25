##XCode8入坑指南
------

> 路径必须/Applications/Xcode.app

```shell
sudo xcode-select -s /Applications/Xcode.app/Contents/Developer
```


------

> 安装pyobjc

``` ruby
sudo -H pip install pyobjc
``` ruby


> 本地编译XCode命令Build


``` 
xcodeBuild clean build -project asura/asura/Unity-iPhone.xcodeproj IPHONEOS_DEPLOYMENT_TARGET="7.0" 2>ios_x8.log -configuration Release CONFIGURATION_BUILD_DIR=build/
```


> 解决Plugin不兼容问题

``` shell
sh -c "$(curl -s https://gist.githubusercontent.com/airmusic/1d52ab0d3ffe2de2172df6d777284167/raw/f5f516ed662c93d39a1ddfde7dacd03205b661b6/UnityPluginFix.sh)"
```