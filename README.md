# amdemos-ios-player
阿里视频云播放器SDK示例代码

## 代码结构
```
├── 根目录                                 // Demo根目录
│   ├── AUIPlayerMain                     // Demo壳组件代码，将其他功能组件UI以列表的形式展示
│   ├── AUIVideoFlow                      // 信息流播放、全屏播放组件代码
│   ├── AUIVideoList                      // 沉浸式短视频组件代码
│   ├── AUIShortEpisode                   // 短剧UI组件代码
│   ├── AUIPlayer.podspec                 // 本地pod文件
│   ├── Example                           // 示例代码工程
│   ├── README.md                         // Readme   

```

## 环境要求
- Xcode 12.0 及以上版本，推荐使用最新正式版本
- CocoaPods 1.9.3 及以上版本
- 准备 iOS 10.0 及以上版本的真机

## 前提条件
获取播放器SDK的License和key，需要包含播放的授权。
参考[获取License](https://help.aliyun.com/zh/vod/developer-reference/license-authorization-and-management)

## 跑通Example Demo

1. 源码下载后，解压进入目录AlivcPlayerDemo
2. 修改Podfile中依赖的播放器SDK为最新版本，版本号参考[iOS播放器SDK](https://help.aliyun.com/zh/vod/developer-reference/release-notes-for-apsaravideo-player-sdk-for-ios)
3. 在Example目录下执行“pod install  --repo-update”，自动安装依赖SDK
4. 打开工程文件“AlivcPlayerDemo.xcworkspace”，修改包Id
5. 在控制台上申请试用License，获取License文件和LicenseKey，如果已有直接进入下一步
6. 把License文件放到AlivcPlayerDemo/目录下，并修改文件名为“license.crt”
7. 把“LicenseKey”（如果没有，请在控制台拷贝），打开“AlivcPlayerDemo/Info.plist”，填写到字段“AlivcLicenseKey”的值中
8. 在真机上编译运行



## 其他

* [播放器SDK](https://help.aliyun.com/zh/vod/developer-reference/apsaravideo-player-sdk/)
* [SDK快速集成](https://help.aliyun.com/zh/vod/developer-reference/quick-integration-1)
* [API说明](https://help.aliyun.com/zh/vod/developer-reference/api-references-ios-player)
* [播放器常见问题](https://help.aliyun.com/zh/vod/support/faq-about-apsaravideo-player/)
* [播放器单点追查](https://help.aliyun.com/zh/vod/user-guide/single-point-tracing)

如果您在使用播放器SDK有任何问题或建议，欢迎通过钉钉搜索群号31882553加入阿里云播放器SDK开发者群。

