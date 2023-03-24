# XiaoFeng.Ftp

![fayelf](https://user-images.githubusercontent.com/16105174/197918392-29d40971-a8a2-4be4-ac17-323f1d0bed82.png)

![GitHub top language](https://img.shields.io/github/languages/top/zhuovi/xiaofeng.ftp?logo=github)
![GitHub License](https://img.shields.io/github/license/zhuovi/xiaofeng.ftp?logo=github)
![Nuget Downloads](https://img.shields.io/nuget/dt/xiaofeng.ftp?logo=nuget)
![Nuget](https://img.shields.io/nuget/v/xiaofeng.ftp?logo=nuget)
![Nuget (with prereleases)](https://img.shields.io/nuget/vpre/xiaofeng.ftp?label=dev%20nuget&logo=nuget)

Nuget：XiaoFeng.Ftp

| QQ群号 | QQ群 | 公众号 |
| :----:| :----: | :----: |
| 748408911  | ![QQ 群](https://user-images.githubusercontent.com/16105174/198058269-0ea5928c-a2fc-4049-86da-cca2249229ae.png) | ![畅聊了个科技](https://user-images.githubusercontent.com/16105174/198059698-adbf29c3-60c2-4c76-b894-21793b40cf34.jpg) |

源码： https://github.com/zhuovi/XiaoFeng.Ftp

教程： https://www.yuque.com/fayelf/xiaofeng

XiaoFeng.Ftp网络库，用两种方式实现了FTP客户端功能，FptRequest及Socket实现。

## XiaoFeng.Ftp

XiaoFeng.Ftp generator with [XiaoFeng.Ftp](https://github.com/zhuovi/XiaoFeng.Ftp).

## Install

.NET CLI

```
$ dotnet add package XiaoFeng.Ftp --version 2.0.0
```

Package Manager

```
PM> Install-Package XiaoFeng.Ftp --Version 2.0.0
```

PackageReference

```
<PackageReference Include="XiaoFeng.Ftp" Version="2.0.0" />
```
Paket CLI

```
> paket add XiaoFeng.Ftp --version 2.0.0
```

Script & Interactive

```
> #r "nuget: XiaoFeng.Ftp, 2.0.0"
```

Cake

```
// Install XiaoFeng.Ftp as a Cake Addin
#addin nuget:?package=XiaoFeng.Ftp&version=2.0.0

// Install XiaoFeng.Ftp as a Cake Tool
#tool nuget:?package=XiaoFeng.Ftp&version=2.0.0
```

# XiaoFeng 类库包含库
| 命名空间 | 所属类库 | 开源状态 | 说明 | 包含功能 |
| :----| :---- | :---- | :----: | :---- |
| XiaoFeng.Prototype | XiaoFeng.Core | :white_check_mark: | 扩展库 | ToCase 类型转换<br/>ToTimestamp,ToTimestamps 时间转时间戳<br/>GetBasePath 获取文件绝对路径,支持Linux,Windows<br/>GetFileName 获取文件名称<br/>GetMatch,GetMatches,GetMatchs,IsMatch,ReplacePatten,RemovePattern 正则表达式操作<br/> |
| XiaoFeng.Net | XiaoFeng.Net | :white_check_mark: | 网络库 | XiaoFeng网络库，封装了Socket客户端，服务端（Socket,WebSocket），根据当前库可轻松实现订阅，发布等功能。|
| XiaoFeng.Http | XiaoFeng.Core | :white_check_mark: | 模拟请求库 | 模拟网络请求 |
| XiaoFeng.Data | XiaoFeng.Core | :white_check_mark: | 数据库操作库 | 支持SQLSERVER,MYSQL,ORACLE,达梦,SQLITE,ACCESS,OLEDB,ODBC等数十种数据库 |
| XiaoFeng.Cache | XiaoFeng.Core | :white_check_mark: | 缓存库 |  内存缓存,Redis,MemcachedCache,MemoryCache,FileCache缓存 |
| XiaoFeng.Config | XiaoFeng.Core | :white_check_mark: | 配置文件库 | 通过创建模型自动生成配置文件，可为xml,json,ini文件格式 |
| XiaoFeng.Cryptography | XiaoFeng.Core | :white_check_mark: | 加密算法库 | AES,DES,RSA,MD5,DES3,SHA,HMAC,RC4加密算法 |
| XiaoFeng.Excel | XiaoFeng.Excel | :white_check_mark: | Excel操作库 | Excel操作，创建excel,编辑excel,读取excel内容，边框，字体，样式等功能  |
| XiaoFeng.Ftp | XiaoFeng.Ftp | :white_check_mark: | FTP请求库 | FTP客户端 |
| XiaoFeng.IO | XiaoFeng.Core | :white_check_mark: | 文件操作库 | 文件读写操作 |
| XiaoFeng.Json | XiaoFeng.Core | :white_check_mark: | Json序列化，反序列化库 | Json序列化，反序列化库 |
| XiaoFeng.Xml | XiaoFeng.Core | :white_check_mark: | Xml序列化，反序列化库 | Xml序列化，反序列化库 |
| XiaoFeng.Log | XiaoFeng.Core | :white_check_mark: | 日志库 | 写日志文件,数据库 |
| XiaoFeng.Memcached | XiaoFeng.Memcached | :white_check_mark: | Memcached缓存库 | Memcached中间件,支持.NET框架、.NET内核和.NET标准库,一种非常方便操作的客户端工具。实现了Set,Add,Replace,PrePend,Append,Cas,Get,Gets,Gat,Gats,Delete,Touch,Stats,Stats Items,Stats Slabs,Stats Sizes,Flush_All,Increment,Decrement,线程池功能。|
| XiaoFeng.Redis | XiaoFeng.Redis | :white_check_mark: | Redis缓存库 | Redis中间件,支持.NET框架、.NET内核和.NET标准库,一种非常方便操作的客户端工具。实现了Hash,Key,String,ZSet,Stream,Log,List,订阅发布,线程池功能; |
| XiaoFeng.Threading | XiaoFeng.Core | :white_check_mark: | 线程库 | 线程任务,线程队列 |
| XiaoFeng.Mvc | XiaoFeng.Mvc | :x: | 低代码WEB开发框架 | .net core 基础类，快速开发CMS框架，真正的低代码平台，自带角色权限，WebAPI平台，后台管理，可托管到服务运行命令为:应用.exe install 服务名 服务说明,命令还有 delete 删除 start 启动  stop 停止。 |
| XiaoFeng.Proxy | XiaoFeng.Proxy | :white_check_mark: | 代理库 | 开发中 |
| XiaoFeng.TDengine | XiaoFeng.TDengine | :white_check_mark: | TDengine 客户端 | 开发中 |
| XiaoFeng.GB28181 | XiaoFeng.GB28181 | :white_check_mark: | 视频监控库，SIP类库，GB28181协议 | 开发中 |
| XiaoFeng.Onvif | XiaoFeng.Onvif | :white_check_mark: | 视频监控库Onvif协议 | XiaoFeng.Onvif 基于.NET平台使用C#封装Onvif常用接口、设备、媒体、云台等功能， 拒绝WCF服务引用动态代理生成wsdl类文件 ， 使用原生XML扩展标记语言封装参数，所有的数据流向都可控。 |


# XiaoFeng.Ftp

## FTP客户端

```csharp
var ftp = new XiaoFeng.Ftp.FtpClient(new XiaoFeng.Ftp.FtpClientConfig
{
     Host= "127.0.0.1",
     Port= 21
});
//上传一个文件
var a = await ftp.PutAsync(@"E://a/a.txt");
//上传一个文件到指定目录
var b = await ftp.UploadFileAsync(@"E://a/a.txt", "/a/a.txt");
//上传一个文件夹到指定目录
await ftp.UploadFolderAsync(@"E://a", "/a");
//下载一个文件到指定目录
var c = await ftp.DownFileAsync(@"/a/a.txt", @"E://a", "a.txt");
//获取文件夹列表
var d = await ftp.GetDirAsync("a");
//获取文件夹列表-详细
var e = await ftp.GetDirListAsync("a");
//获取文件详细信息
var f = await ftp.GetFileInfoAsync("a/a.txt");
//获取文件大小
var g = await ftp.GetFileSizeAsync(@"a/a/txt");
//改变文件目录
var h = await ftp.ChangeDirectoryAsync("/b");
//删除文件夹
var i = await ftp.DeleteAsync("a");
//删除文件
var j = await ftp.DeleteAsync("a/a.txt");
//当前目录
var k = ftp.RemoteDirectory;
```

# 作者介绍

* 网址 : http://www.fayelf.com
* QQ : 7092734
* EMail : jacky@fayelf.com