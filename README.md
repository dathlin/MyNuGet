# MyNuGet
一个基于本地的NuGet服务器，用于本地或是公司的.net的包管理器。

NuGet.Server相关的组件版权归原作者所有。

# 搭建流程
## 1.安装IIS和ASP.NET支持
运行控制面板，打开高级选项，勾选IIS核心，勾选ASP.NET支持。
## 2.配置网站
打开控制面板的管理工具，里面有IIS管理器，新建网站，配置端口，虚拟目录。启动网站。
## 3.下载nuget package explorer
这个一个打包dll成negut文件的应用程序，项目地址为：
[https://github.com/NuGetPackageExplorer/NuGetPackageExplorer](https://github.com/NuGetPackageExplorer/NuGetPackageExplorer)

可用于下载上传相关的nuget包。
## 4.配置visual studio的nuget参数
新增一个服务器来源，比如 ***http://127.0.0.1:80/nuget*** ，具体的值根据网站创建的信息来。
## 5.打开visual studio的nuget包管理器
现在可以浏览自己的服务器上的所有的组件包了，还可以下载，支持更新。