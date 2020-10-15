# URLSchemes

Loon 支持 URL Schemes，可结合其他工作流使用

## URL

```
开启或关闭 Loon

loon://switch

导入配置

loon://import

打开 Loon 配置文件

loon://editconfig

打开最近请求

loon://requestLists

打开日志

loon://LogLists
```

## 举例

若用户想导入配置，可以使用 loon://import?sub=url （URL为 Urlencode 之后的字符串）

loon://import?sub=https%3A%2F%2Floon.now.sh%2Flazy-config%2Fdefault