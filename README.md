# XiaoFeng.Ftp

![fayelf](https://user-images.githubusercontent.com/16105174/197918392-29d40971-a8a2-4be4-ac17-323f1d0bed82.png)

![GitHub top language](https://img.shields.io/github/languages/top/zhuovi/xiaofeng.ftp?logo=github)
![GitHub License](https://img.shields.io/github/license/zhuovi/xiaofeng.ftp?logo=github)
![Nuget Downloads](https://img.shields.io/nuget/dt/xiaofeng.ftp?logo=nuget)
![Nuget](https://img.shields.io/nuget/v/xiaofeng.ftp?logo=nuget)
![Nuget (with prereleases)](https://img.shields.io/nuget/vpre/xiaofeng.ftp?label=dev%20nuget&logo=nuget)

Nuget：XiaoFeng.Ftp

QQ群号：748408911 

QQ群二维码： 

![QQ 群](https://user-images.githubusercontent.com/16105174/198058269-0ea5928c-a2fc-4049-86da-cca2249229ae.png)

公众号： 

![畅聊了个科技](https://user-images.githubusercontent.com/16105174/198059698-adbf29c3-60c2-4c76-b894-21793b40cf34.jpg)

源码： https://github.com/zhuovi/XiaoFeng.Ftp

教程： https://www.yuque.com/fayelf/xiaofeng

XiaoFeng.Ftp网络库，用两种方式实现了FTP客户端功能，FptRequest及Socket实现。

## XiaoFeng.Ftp

XiaoFeng.Ftp generator with [XiaoFeng.Ftp](https://github.com/zhuovi/XiaoFeng.Ftp).

## Install

.NET CLI

```
$ dotnet add package XiaoFeng.Ftp
```

Package Manager

```
PM> Install-Package XiaoFeng.Ftp
```

PackageReference

```
<PackageReference Include="XiaoFeng.Ftp" Version="2.0.0" />
```

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