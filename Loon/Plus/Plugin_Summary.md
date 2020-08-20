# 什么是插件

- 官方解析：

  - TestFlight(192)：添加Plugin插件，一个插件就是按功能区分的子配置，格式个(跟)profile配置文件相同，plugin中的配置优先级最高，目前暂时支持 `[URL Rewrite]` 、 `[Script]` ， `[MITM]` 模块，后续会扩展更多模块，相关配置格式见example样例配置，相关plugin格式详见：[格式](https://raw.githubusercontent.com/Loon0x00/LoonExampleConfig/master/Plugin/Plugin_Example.plugin)
  
  - TestFlight(193)：支持 `[Rule]` 模块，策略可设置为DIRECT,REJECT,PROXY，其中PROXY为用户在app中手动映射的策略，rule后不跟随策略默认使用PROXY，相关样例配置详见：[格式](https://github.com/Loon0x00/LoonExampleConfig/blob/master/Plugin/Plugin_Example2.plugin
  
- 小白理解：可以将插件理解成一个残疾版的配置文件，通过读取 URL 内容，自动识别相应模块下的代码片段，批量在 Loon 配置文件内插入大量的代码片段，且执行优先级最高

## 关于添加插件中对 URL 的要求及内容格式要求

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 关于添加插件中对 URL 的要求、内容格式要求、其他一系列问题，请点击 [这里](https://github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin_Format.md) 跳转到 `添加插件中对 URL 的要求及内容格式要求` 教程

# 多说几句

- 虽然支持 `[Script]` 模块，但是不建议将**获取cookie类脚本**、**签到类脚本**的脚本配置代码写入插件文件内，原因是折腾用户

- 建议将类似于 `京东、淘宝历史价格脚本` 的脚本配置代码写入插件文件内，因为此类脚本不会有弹窗提醒，也不需要修改执行时间

# 参考

- [TestFlight(192)](https://t.me/LoonNews/187)

- [TestFlight(193)](https://t.me/LoonNews/194)
