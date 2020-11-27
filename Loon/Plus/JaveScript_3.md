# 高级

JaveScript API example


### 可以查看大神写的[教程](https://jidesheng6.github.io/loonapidoc.html)，感谢这位大神！

### 一、

```
/*
 * Loon script example
 */
//log
console.log('This is a log');

//http get params
var params = {
    url:"https://api.example.com/post",
    header:{
        Host:"api.example.com",
        Content-Type: "application/json",
    },
    body:"string"
}

$httpClient.get('https://example.com/index',function(error, response, data){
    console.log(response);
});

//http get
$httpClient.get(params,function(error, response, data){
    console.log(response);
});

//http post
$httpClient.post(params,function(error, response, data){
    console.log(response);
});

//notification
$notification.post('title<String>', 'subtitle<String>', 'body<String>')

//persistentStore
$persistentStore.write('data<String>', 'key<String>')
$persistentStore.read('key<String>')
```

### 二、cron.js
```
/*
*/

console.log('Start JS');
$notification.post("title","subtitle","body");
$done();
```

### 三、netChanged.js
```
  
/*
network-changed script-path=https://raw.githubusercontent.com/Loon0x00/LoonExampleConfig/master/Script/netChanged.js
*/

//获取Loon的相关配置，返回为json格式
var confStr = $config.getConfig()
console.log(confStr)

var conf = JSON.parse(confStr)
if (conf.ssid == "your ssid name") {
    /*
    设置全局运行模式
    0:Global Direct
    1:By Rule
    2:Global Proxy
    */
    $config.setRunningModel(0)
    //设置select策略组所对应的策略，子策略不存在时将保持原先的策略不变
    $config.setSelectPolicy("⛔ 广告拦截","DIRECT")
    $notification.post("Network changed","Change Running Model to Global Direct","⛔ 广告拦截 to DIRECT")
} else {
    $config.setRunningModel(1)
    $config.setSelectPolicy("⛔ 广告拦截","REJECT")
    $notification.post("Network changed","Change Running Model to Filter by rule","⛔ 广告拦截 to REJECT")
}

//一次性同时设置多个策略组的策略
$config.setSelectPolicy(["国外网站","广告拦截","谷歌服务"],["HK Node 1","REJECT","节点选择"])

//获取相关策略的子策略，json格式
var subPolicys = $config.getSubPolicys("节点选项")
console.log(subPolicys);
```

# 参考

- [Loon0x00](https://github.com/Loon0x00/LoonExampleConfig/tree/master/Script)
