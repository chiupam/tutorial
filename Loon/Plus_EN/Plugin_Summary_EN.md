# What is a plugin

 -Official analysis:

  - [TestFlight(192)](https://t.me/LoonNews/187): add Plugin, a plugin is a sub-configuration distinguished by function, the format is the same as the profile configuration file, and the configuration in the plugin takes precedence The highest level, currently supports `[URL Rewrite]`, `[Script]`, `[MITM]` modules for the time being. More modules will be expanded in the future. For related configuration formats, please refer to example configuration. For related plugin formats, please refer to: [format ](https://raw.githubusercontent.com/Loon0x00/LoonExampleConfig/master/Plugin/Plugin_Example.plugin)
  
  - [TestFlight(193)](https://t.me/LoonNews/194): Support the `[Rule]` module, the strategy can be set to DIRECT, REJECT, PROXY, where PROXY is the strategy manually mapped by the user in the app , Without following the policy after the rule, PROXY is used by default. For the related sample configuration, please refer to: [format](https://raw.githubusercontent.com/Loon0x00/LoonExampleConfig/master/Plugin/Plugin_Example2.plugin)
  
  
- Xiaobai understands: The plug-in can be understood as a disabled version of the configuration file, by reading the URL content, the code snippets under the corresponding module are automatically recognized, and a large number of code snippets are inserted into the Loon configuration file in batches, and the execution priority is the highest

## Regarding URL requirements and content format requirements in adding plugins

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Regarding URL requirements, content format requirements, and a series of other questions in adding a plug-in, please click [here](https: //github.com/chiupam/tutorial/blob/master/Loon/Plus/Plugin_Format.md) Jump to the `Add plug-in URL requirements and content format requirements` tutorial

# Say a few more words

- Although the `[Script]` module is supported, it is not recommended to write the script configuration code of the **check-in script** into the plug-in file, because adding scripts in this way does not allow users to modify the script execution time

- It is recommended to write script configuration code similar to `Jingdong, Taobao historical price script` into the plug-in file, because such scripts will not have pop-up reminders, and there is no need to modify the execution time

# Reference

- [TestFlight(192)](https://t.me/LoonNews/187)

- [TestFlight(193)](https://t.me/LoonNews/194)