# CleverQQHTTP
一款跨平台的CleverQQ插件

## CleverQQHTTP用法

[基本使用](https://github.com/vaemc/CleverQQHTTP/wiki/%E5%9F%BA%E6%9C%AC%E4%BD%BF%E7%94%A8)

[C#示例代码](https://github.com/vaemc/CleverQQHTTP/wiki/C%23%E7%A4%BA%E4%BE%8B)

[Java示例代码](https://github.com/vaemc/CleverQQHTTP/wiki/Java%E7%A4%BA%E4%BE%8B)

[Python示例代码](https://github.com/vaemc/CleverQQHTTP/wiki/Python%E7%A4%BA%E4%BE%8B)

[微信小程序示例代码](https://github.com/vaemc/CleverQQHTTP/wiki/%E5%BE%AE%E4%BF%A1%E5%B0%8F%E7%A8%8B%E5%BA%8F%E7%A4%BA%E4%BE%8B)

[易语言示例代码](https://github.com/vaemc/CleverQQHTTP/wiki/%E6%98%93%E8%AF%AD%E8%A8%80%E7%A4%BA%E4%BE%8B)

[E4A示例代码](https://github.com/vaemc/CleverQQHTTP/wiki/E4A%E7%A4%BA%E4%BE%8B)



* 必须以管理员身份运行CleverQQ，然后启动CleverQQHTTP插件。

* 所有的API的参数均以Json格式Post提交

* 例如http://localhost:8087/api/Api_SendMsg 其中`Api_SendMsg`为接口名称，他需要的参数是机器人的QQ号，以Json的形式提交参数
`{"RobotQQ":"1740531365"}` 具体的接口和对应的参数名可以查看官方API文档。
* ***API的名称和参数名称完全和官方一致。***

* 要在小程序使用CleverQQHTTP，需勾选 **启用HTTPS** ，并申请SSL证书，证书名后缀 **pfx**。将证书放在CleverQQ的 **运行目录** ，注意是CleverQQ的 **运行目录** 不是插件的目录！

* 接收QQ消息需要自己实现Socket客户端链接设置好的端口。接收到消息后数据以Json的格式发送给客户端。

* 由于CleverHTTP还在测试阶段，很多异常都没有捕捉。只要正确使用（post数据对应API的参数、URL的API地址对应官方的API名称……）就不会引起插件崩溃。注意只要一但发送请求后没有响应（也就是发生了错误），就应当重启CleverQQ重新开启插件。


![kVLuQS.jpg](https://s2.ax1x.com/2019/01/24/kVLuQS.jpg)

![kVqi40.jpg](https://s2.ax1x.com/2019/01/24/kVqi40.jpg)


