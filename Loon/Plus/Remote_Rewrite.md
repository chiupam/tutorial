# 复写

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在收到 http 请求时，Loon 会使用请求的 url 去寻找匹配的 url rewrite，一个 URL Rewrite 会根据匹配的规则替换或者修改 HTTP 请求中的 url，或者替换请求响应体。 

## 格式要求

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 一个 URL Rewrite 分为三部分：正则表达式，替换内容，rewrite类型 

### 例如

```
https?://(www.)?g.cn https://www.google.com 302
```

## 支持类型

- header 

  - 请求头中匹配的host字段将会被替换内容所替换

- reject 

  - 直接拒绝请求

- 302 
  
  - 返回302响应

- 307 

  - 返回307响应