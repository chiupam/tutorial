# 什么是插件

- 官方解析：

  - 添加Plugin插件，一个插件就是按功能区分的子配置，格式个(跟)profile配置文件相同，plugin中的配置优先级最高，目前暂时支持 `[URL Rewrite]` 、 `[Script]` ， `[MITM]` 模块，后续会扩展更多模块，相关配置格式见example样例配置，相关plugin格式详见：[格式](https://raw.githubusercontent.com/Loon0x00/LoonExampleConfig/master/Plugin/Plugin_Example.plugin)
  
  - 后续支持了 `[Rule]` 模块
  
- 小白理解：可以将插件理解成一个残疾版的配置文件，为用户定制添加
