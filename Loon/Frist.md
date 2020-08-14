# 首次使用 Loon

此教程仅让首次使用 Loon 的用户成功科学上网，更多详细教程后面会更新，敬请期待

## 一、通过 URL 下载功能下载一份简易版配置

先复制右侧这串地址：https://raw.githubusercontent.com/chiupam/Proxy/master/Loon/Loon_example.conf

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/peizhi.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 下拉找到并点击 `从URL下载`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `添加`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL_1.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 将上面复制/拷贝的地址粘贴在下图的位置

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL_2.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `确定`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/URL_3.png)

## 二、配置证书（如果中途操作停止可能导致CA证书不一致，此时请删除证书重新操作此步骤）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏，下拉找到并点击 `证书管理`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/zhengshuguanli.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `生成新的CA证书`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `安装CA证书`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 在跳转出来的页面中点击 `允许`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开手机设置并点击 `已下载描述文件`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `安装` 后，应该会出现验证的步骤，按步骤即可

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_5.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 回到手机设置并点击 `通用` ，然后点击 `关于本机`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_6.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `证书信任设置`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_7.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击按钮使 `灰色按钮` 变成`绿色按钮`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/mitm_8.jpg)

## 三、添加订阅节点 (第三步与第四步必须连贯做)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏，点击 `订阅节点`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Proxy.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 左滑 `机场订阅` （使用本教程提供的URL下载配置才会有如下图所示的 `机场订阅` ，如果导入其他懒人配置，请根据懒人配置内说明操作此步骤）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Proxy_2.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `编辑`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Proxy_3.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 先点击  `URL` 右侧，使得 `X` 出现

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Proxy_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 将机场订阅复制并粘贴到 `URL` 右侧位置，最后点击 `保存`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Proxy_5.jpg)

## 四、筛选订阅节点 (在此之前必须完成第三步)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击下方 `配置` 栏，点击 `筛选订阅节点`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Filter.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `订阅筛选` （使用本教程提供的URL下载配置才会有如下图所示的 `订阅筛选` ，如果导入其他懒人配置，请根据懒人配置内说明操作此步骤）

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Filter_1.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击下图所示区域

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Filter_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `X` 符号以删除 `.*` 

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Filter_3.jpg)

### 先学习正则表达式再往下看

- (A).*(B) or (A.*B|B.*A)
 - 节点名既有A又有B，例如 `(香港).*(IPLC).*(x1)`
- (A)|(B) or ^.*(A|B)
 - 节点名有A或者B，例如 `(IPLC)|(IEPL)`
- ^((?!A).)*$
 - 节点名不含有 A，例如 `^((?!x1.5).)*$`
- (?!.*(A)).*(B) or ^(?!.*?A).*B
 - 节点名不含有 A同时含有 B，例如 `(?!.*(x1.5)).*(香港)`

### 看懂了再进行下一步

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 输入正则表达式

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Filter_4.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 检查筛选后的节点

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Remote_Filter_5.jpg)

## 五、启动 Loon 连接（此步是很多新用户最容易遗漏的一个步骤）

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击右上角 `Start`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/START.jpg)

## 六、选择策略以及子策略组的节点选择

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 打开 Loon 并点击 `策略组`

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 点击 `𝐏𝐫𝐨𝐱𝐲` 并从下级菜单中选择

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_1.png)

- 如果选择了 手动选择 策略组请进行下列操作

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Proxy_Group_select.jpg)

- 如果选择了 优选地策略 or 健康检测 则不需要进行任何操作

## 完成~~~

# 逻辑图帮助理解

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Frist_end.png)

# 欢迎进入 Loon 官方 Telegram 频道 点击 [这里](https://t.me/Loon0x00) 跳转

