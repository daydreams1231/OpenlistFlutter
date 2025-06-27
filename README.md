## 单纯Fork了原仓库, 将所有alist相关的库换成了openlist的, 如果你需要fork本仓库请注意:
去Settings -> Secrets and variables -> Actions -> Repo secret添加你自己的secret <br>
ALIAS_NAME  ALIAS_PASSWORD  KEY_PASSWORD  KEY_STORE  <br>
其中KEY_STORE存储前三项对应的jks签名文件的base64编码<br>

貌似OpenList仓库还有点问题, 使用go get github.com/OpenListTeam/OpenList/v3/cmd出现: <br>
```
go: github.com/OpenListTeam/OpenList/v3@v3.45.0: parsing go.mod:
        module declares its path as: github.com/alist-org/alist/v3
                but was required as: github.com/OpenListTeam/OpenList/v3
```
等以后再修吧<br>
[![Release](https://github.com/jing332/AListFlutter/actions/workflows/release.yaml/badge.svg)](https://github.com/jing332/AListFlutter/actions/workflows/release.yaml)
[![Test](https://github.com/jing332/AListFlutter/actions/workflows/build.yaml/badge.svg)](https://github.com/jing332/AListFlutter/actions/workflows/build.yaml)
[![CheckAList](https://github.com/jing332/AListFlutter/actions/workflows/sync_alist.yaml/badge.svg)](https://github.com/jing332/AListFlutter/actions/workflows/sync_alist.yaml)

#### 🚩　[FRP](https://github.com/fatedier/frp) 安卓版本：https://github.com/jing332/FrpAndroid
#### 🚩　[AListAndroid](https://github.com/jing332/AlistAndroid) Compose版本，已停更

# AListFlutter

AListFlutter是一个基于AList的Android服务端，使用Google Flutter作为UI框架。

> [Github Actions](https://github.com/jing332/AListFlutter/actions/workflows/sync_alist.yaml)
> 每日早晚五点钟检查最新的 [AList](https://github.com/alist-org/alist/releases)
> 并自动构建APK，发布到 [Release](https://github.com/jing332/AListFlutter/releases)
> 中，您只需耐心等待片刻并在应用内检查更新即可。

<img src="./images/alist.jpg" height="150px">

### Bug
- Android4.4闪退 https://github.com/jing332/AListFlutter/issues/5
- 部分设备无法添加本地存储 https://github.com/jing332/AListFlutter/issues/2

### 关于IOS
理论上 [Gomobile](https://pkg.go.dev/golang.org/x/mobile/cmd/gomobile?utm_source=godoc#hdr-Build_a_library_for_Android_and_iOS) 支持IOS，但由于本人无IOS相关开发设备，故无法支持。

# Download

- [Github Action (DEV)](https://github.com/jing332/AListFlutter/actions/workflows/build.yaml) 开发版

