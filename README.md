# PackageApplication
xcrun: error: unable to find utility "PackageApplication", not a developer tool or in PATH

后面根据对比发现新版的Xcode少了这个PackageApplication（转注：PackageApplication在前几个版本已被标识为废弃，在8.3版本彻底移除了）

先去找个旧版的Xcode里面copy一份过来

放到下面这个目录：

/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/usr/bin/

然后执行命令：

sudo xcode-select -switch /Applications/Xcode.app/Contents/Developer/

chmod +x /Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/usr/bin/PackageApplication

2句分开执行

最后附上PackageApplication下载地址：

