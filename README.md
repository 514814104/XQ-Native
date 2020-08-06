# XQ-Native
让XQ先驱机器人兼容大部分CQ插件

## 快速使用

1. 下载 [Native.XQ.Lib] 插件 ， 放入Plugin（先驱机器人插件目录）
2. 下载 [XQNative] 插件 ， 放入Plugin（先驱机器人插件目录）
3. 下载伪造CQP.dll [CQP.dll] ， 放入先驱目录下 （和 先驱.exe 同目录）
4. 启动先驱机器人，在插件管理处启动 Native.XQ.Lib 和 XQNative 插件
5. 关闭先驱机器人，创建目录 CQPlugins 
5. 移动原酷q插件的dll和json文件到   CQPlugins\应用名\ 

呈现目录结构为

>> └─先驱机器人主目录
>>     │  CQP.dll // XQ Native Bridge
>>     │
>>     ├─CQPlugins // 被XQ-Native加载的所有CQ插件
>>     │      ├─com.example.cqapp1 //某个目录
>>     │      │        │─ app.dll
>>     │      │        └─ app.jso
>>     │      │─com.example.cqapp2 //某个目录
>>     │      │        │─ app.dll
>>     │      │        └─ app.json
>>     │      └─com.example.cqapp3 //某个目录
>>     │               │─ app.dll
>>     │               └─ app.json
>>     └─Plugin // 插件文件夹
>>             XQNative.XQ.dll // XQ-Native桥接插件
>>             Native.XQ.Lib.XQ.dll // Native发送消息兼容插件