# 云游戏 Web SDK demo

这个开源项目展示了火山引擎云游戏 Web SDK 的以下功能：

1. 开始游戏和结束游戏

方便用户快速接入云游戏 Web SDK。

## 运行示例程序

1. 将 Web SDK demo 代码下载到本地；
2. 前往火山引擎 [云游戏文档中心]( https://www.volcengine.com/docs/6512/75594)，下载 Web SDK；解压后将其复制到 `lib` 文件夹下，并重命名为 `veGameSDK-Web.js`；
3. 在 `config.js` 中补全以下配置信息：

```js

// 实例化 veGameSDK 的参数
const initConfig = {
    userId: ''
};

// 调用 veGameSDK.start 的参数
// 以下只列出调用参数的必传参数，更多参数参考 Web SDK 的使用文档
const startConfig = {
    gameId: '',
    token: {
        CurrentTime: '',
        ExpiredTime: '',
        SessionToken: '',
        AccessKeyID: '',
        SecretAccessKey: ''
    },
    roundId: '',
    rotation: 'landscape', // landscape：横屏启动; portrait：竖屏启动
};

```

3. 在浏览器中打开 `index.html` 文件；
   
4. 点击开始游戏。

## 参考资料

客户端 SDK 下载：https://www.volcengine.com/docs/6512/75597

注：如果不能访问以上链接，请参考 [开通云游戏服务](https://www.volcengine.com/docs/6512/75577) 说明文档。
