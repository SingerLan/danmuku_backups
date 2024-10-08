>问题或建议，请加QQ群留言。**199580494**

**不看弹幕的请绕行，请阅读下方文本熟悉使用方法。**
## 一、简介
- 支持自定义弹幕
- 支持弹幕时间轴调整
- 支持自定义背景api
- v0.2版本 ~~根据OK影视2.3.4修改~~ 
- v0.4版本 ~~根据OK影视2.3.9修改~~ 
- 根据OK影视2.4.0修改 <span style="color: red">新</span>
-  v0.2版本 ~~修改OK影视2.3.4弹幕越播越快的bug~~
- 适配gitee私有仓库 <span style="color: red">新</span>
- 适配弹幕服务解析 <span style="color: red">新</span>
### 1.1 更新内容：
#### 20240625：
1. 提高弹幕加载速度。
2. 适配影视2.4.0。
3. 修改解析配置。
4. 修复影视2.4.0语法错误。
#### 20240628：
1. 修改集数匹配规则
#### 20240711
1. 弹幕文件更改为压缩包，网络访问更快

## 二、功能介绍
### 2.1 自定义弹幕
1. 设置->填入自定义弹幕地址：弹幕json文件
2. 播放带弹幕的资源
3. 如果开启自定义则会根据“弹幕json文件”匹配新的弹幕
### 2.2 自定义背景api
例如：https://raw.githubusercontent.com/SingerLan/json/master/random.png
程序会将random随机替换成0～9任意数字。
>如随机数字是2，实际的背景图是https://raw.githubusercontent.com/SingerLan/json/master/2.png
>![image](https://github.com/SingerLan/danmuku/assets/44799711/9fff238b-8cdd-4dd0-b143-01121598332a)
### 2.3 弹幕时间轴调整
因资源不同，弹幕与视频的时间可能不匹配，故增加时间轴  
- TV：设置->弹幕设置->可调整正负600秒
- 手机：弹幕设置弹窗->可调整正负600秒(可能需要退出视频，重新进入，没有测试过)

### 2.4 gitee私有仓库适配 <span style="color: red">新</span>
在弹幕URL地址处将?access_token=*** 加载最后端


### 2.5 弹幕服务器解析 <span style="color: red">新</span>
1、在弹幕URL地址处将?danmaku_url=*** 加载最后端
2、将解析地址填到json文件里：如玫瑰的故事.json

## 三、弹幕json文件介绍
```
[{"name":"玫瑰的故事","url":"https://raw.githubusercontent.com/SingerLan/danmuku/main/玫瑰的故事"},
[{"name":"谍影重重","url":"https://raw.githubusercontent.com/SingerLan/danmuku/main/谍影重重/谍影重重.xml"}]]
```
<span style="color: red">注意:剧集的url是文件夹地址，电影的url是文件地址</span>  
<span style="color: orange">注意:剧集文件夹内的文件名必须：E01.xml，E02.xml，E03.xml...</span>  
<span style="color: blue">注意:剧集电影的文件夹或电影的"name"必须与播放的剧集电影相同，否则无法正确匹配</span>  

## 四、问题说明

v0.2版本  ~~4.1 为什么在2.3.4基础上修改？~~  
v0.2版本  ~~OK一直不更新release代码，2.3.7个人感觉播放器解码有点问题。催ok大佬更新~~  
### 4.1 在2.3.9基础上修改

### 4.2 为什么修改自定义背景api？
  想用自己的图片，自己还没有服务器，随机图片只能这么写了，下面是我用的api地址
  > https://raw.githubusercontent.com/SingerLan/json/master/random.png  
  random是固定的  
  自己做格式为：https://*****/random.png  
  $\color{red} {注意:不想使用只能推送壁纸，填其它格式的地址无效} $

v0.2版本 ~~4.3 为什么要替换已经有弹幕的节点，而不是所有资源都加上弹幕？~~  
v0.2版本 ~~因为只有带弹幕的节点会返回当前播放的视频信息，没有弹幕的节点没发匹配。~~  
v0.2版本~~但现在有屏幕title，新版应该可以获取了，不清楚ok大佬没更新代码。~~  
v0.2版本 ~~更新代码后看情况修改~~  
### 4.3 所有资源都加可以上弹幕  <span style="color: red">新</span>

### 4.4 手机弹幕时间轴调整不能实时？
手机：弹幕设置弹窗->可调整正负600秒(可能需要退出视频，重新进入，没有测试过)

## 五、其它说明  
- OK更新本版本相关内容，将删除该app。 ：**1、已删除v0.2弹幕同步的代码**
- 关注Ok公众号，获取OK接口，资源丰富。
- 可直接使用我已经配好的“弹幕json文件”，但个人采集的弹幕有限，“弹幕json文件”里没有的资源可以等我采集，也可以大家采集好发我，我把弹幕部署上
> 地址：https://raw.githubusercontent.com/SingerLan/danmuku/main/home.json  
>  <span style="color: red">新</span>国内地址：https://raw.gitcode.com/baidu_38752858/danmuku/raw/main/home.json
- 支持本地文件：file://
## 六、收费
  本人搜集、收藏B站下架视频弹幕1G以上，韩剧弹幕500M以上，如需要可联系作者（付费）。
  除以上其它内容开放，

## 七、下载  
https://github.com/SingerLan/danmuku/releases   
https://www.123pan.com/s/Fx2YTd-PXJfv.html  
## 八、鸣谢
  弹幕爱好者们