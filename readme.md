# 《战斗，爽！》模组开发手册

## 前言

代码编辑器首选Visual Studio

## 模组开发环境配置

### Visual Studio Code

进入官网下载vscode：[Download Visual Studio Code - Mac, Linux, Windows](https://code.visualstudio.com/Download)

选择左侧拓展按钮，安装汉化插件：

![image-20240722180617913](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722180617913.png)

然后安装vscode-solution-explorer

![image-20240722180643601](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722180643601.png)

期间可能会提示让你下载其它插件，都下载下来即可

如果左侧工具栏有这个图标证明你vscode-solution-explorer安装成功了

![image-20240722180805533](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722180805533.png)

点击此图标后，在最上方点击这个文件夹的图标

![image-20240722180939289](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722180939289.png)

打开附件中的.sln文件

![image-20240722181012378](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722181012378.png)

对此图标右键选择Add new project

![image-20240722181342523](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722181342523.png)

中间的窗口一直往下滑，选择类库

![image-20240722181419440](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722181419440.png)

选择C#

![image-20240722181446713](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722181446713.png)

输入项目名称

![image-20240722181532646](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722181532646.png)

接下来会让你输入主文件夹名称，这边建议和项目名一直，也就是输入项目名称之后按两下回车即可

如果最下方终端没有报错即可进行下一步

![image-20240722181734181](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722181734181.png)

编辑你项目根目录中的.csproj文件，添加如下字段(可以到Example文件夹里复制)

![image-20240722181955231](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722181955231.png)

然后把Example文件夹中的Library文件夹（或者附件的Library文件夹）复制到你的项目根目录下

对你的项目右键点击Build按钮

![image-20240722182334236](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722182334236.png)

在项目根目录下的bin/Debug/net8.0文件夹中有个【项目名.dll】的文件

这个就是你的模组dll文件了

如果没有或者终端报错证明模组开发环境配置失败

### Visual Studio

下载软件本体，选择社区版即可

[下载 Visual Studio Tools - 免费安装 Windows、Mac、Linux (microsoft.com)](https://visualstudio.microsoft.com/zh-hans/downloads/)

双击安装程序，选择以下配置

![image-20240722182743944](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722182743944.png)

然后安装即可

(若觉得此文档的安装教程并不详细可以百度自行搜索Visual Studio C#开发环境配置教程)



安装完成之后直接双击附件的.sln文件打开项目![image-20240722183034748](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722183034748.png)

在右侧解决方案资源管理器中找到FightAwesomeEngin解决方案然后对其右键选择添加，新建项目

![image-20240722183300260](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722183300260.png)

选择类库即可

![image-20240722183418684](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722183418684.png)

根据提示输入项目名，然后选择Net8.0框架

选择依赖项右键添加项目引用

![image-20240722183644847](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722183644847.png)

点击浏览

![image-20240722183724692](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722183724692.png)

框选附件中Library文件夹中的所有.dll文件

![image-20240722183828298](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722183828298.png)

点击确定

右键你的项目点击生成按钮，如果没有报错代表模组开发环境配置完毕

![image-20240722184007769](C:\Users\34845\Desktop\模组开发手册\assets\image-20240722184007769.png)

在项目根目录下的bin/Debug/net8.0文件夹中有个【项目名.dll】的文件

这个就是你的模组dll文件了

如果没有或者终端报错证明模组开发环境配置失败