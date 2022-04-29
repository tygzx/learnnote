- 分析的app:得物
    - 版本:4.90.0
    - 我们的目标:推荐页的tab 页面

- 第一步:开始抓包
    - 上charles
        - charles 没找到包，
        - 一般android 的开发人员用的okhttp,上frida
        的hookokhttp 的脚本. 脚本来自.<a> https://github.com/siyujie/OkHttpLogger-Frida</a>  
        如下图所示。
        ![image.png](https://upload-images.jianshu.io/upload_images/1250148-2a9de00b7053e4a8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

        - 调用AESEncrypt.encode(DuHttpConfig.f21570c, sb2)
        其中sb2 通过frida hook 得到一个示例值是
        loginTokenplatformandroidtimestamp1651026050145uuid30c7ecc9c3942f48v4.91.1
        返回的参数是:H386HCRD4ndywJq709EsgPqzHgcxbT3IugXCD4BRuIfh1peDzSOrIx1A7M0iJwzLwS0wpuyJGYQswS8FfMZjRE8YPuaVLpZ7Y8B/+6UHqRPVJaZ/I9hE+dLK4B/lVm1xPIt26qjGAZdJZtdWPn/tsw==