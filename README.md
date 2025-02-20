简体中文 | [English](README_EN.md)

# MODNET-Matting-tool
基于深度学习的抠图工具C#推理工具  
[[`Paper`](https://arxiv.org/pdf/2011.11961.pdf )]  


关注微信公众号：**人工智能大讲堂**    
<img width="180" src="https://user-images.githubusercontent.com/18625471/228743333-77abe467-2385-476d-86a2-e232c6482291.jpg">  
后台回复【mat】获取安装包以及模型文件  

## 支持多种文件类型</h2>  
 文件->图像文件 加载本地图像文件  
 文件->截图  
 文件->剪切板  
 文件->视频  为了效率目前Fps为2，即每秒两帧

 <img width="500" src="https://user-images.githubusercontent.com/18625471/258716872-9098bd15-165b-41b8-9fe4-77cc7d42a94c.png">  
 
 ## 支持背景替换</h2>  
 背景->背景颜色 背景替换为纯色  
 <img width="500" src="https://user-images.githubusercontent.com/18625471/258718249-be1ccc3b-bc17-4b52-b77b-42761a75f5e6.png">  
 背景->背景图像  将背景替换为图像  
 <img width="500" src="https://user-images.githubusercontent.com/18625471/258718270-b71ece79-cfc6-408c-a089-12e3eb807085.png">  

  ## 支持多种保存选择</h2>  
  保存->保存整体  前景+背景  
  <img width="300" src="https://user-images.githubusercontent.com/18625471/258719054-bf497476-c953-420f-a0a3-228545c7a60d.png">   
  
  保存->保存前景  只保存前景  
  <img width="300" src="https://user-images.githubusercontent.com/18625471/258719046-f863bb9e-7334-45cd-ab7c-2b33aa044810.png">   
  保存的图像和视频都在exe所在路径下。  
  


 ## 源码编译</h2>  
1. 下载源码到本地  
1. 解压Model目录
1. Visual Studio打开.sln项目解决方案  
1. 安装Nuget包  
    1. 在Visual Studio中，鼠标右键单击项目并选择“管理NuGet程序包”。  
    1. 在“NuGet包管理器”窗口中，选择“安装”选项卡。
    2. 点击“还原”按钮。
2. 运行程序

注意：有时前景图像中可能带有一些碎片，可以使用OpenCV最大连通域算法去掉小的碎片。
