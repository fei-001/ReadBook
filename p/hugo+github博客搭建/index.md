+++
title = 'Hugo+github博客搭建'
date = 2025-04-27T15:58:34+08:00
draft = true

+++

## hego+github实现个人博客部署

**参考B站博主Letere-莱特雷**

### 环境准备

[Release v0.131.0 · gohugoio/hugo](https://github.com/gohugoio/hugo/releases/tag/v0.131.0)

![image-20250427101517633](index.assets/image-20250427101517633.png)

 **从hugo目录进入cmd并创建一个dev文件夹**

```
hugo new site dev
```

![image-20250427101823336](index.assets/image-20250427101823336.png)

可参考：

![image-20250427102059548](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427102059548.png)

```
cd dev
```

**由于没有配置全局，所以将hugo.exe复制到dev文件夹内**

![image-20250427102354001](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427102354001.png)

### 挑选主题

https://themes.gohugo.io

#### 选择合适的

![image-20250427103510548](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427103510548.png)

![image-20250427103535149](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427103535149.png)

#### 选择版本：

![image-20250427103643012](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427103643012.png)

#### 下载源码：

![image-20250427103613286](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427103613286.png)

#### 解压到对应的目录下：

![image-20250427104038580](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427104038580.png)

### 文件配置

#### 在解压后的文件中进行以下操作

![image-20250427104739053](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427104739053.png)

#### 将以下两个文件复制到dev目录下并删除hugo.toml

![image-20250427104912321](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427104912321.png)

![image-20250427104944423](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427104944423.png)

#### 删掉以下文件

![image-20250427105103117](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427105103117.png)

#### 修改文件名将版本号删掉

![image-20250427105329179](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427105329179.png)

#### 启动测试一下

```
hugo server -D 
```

![image-20250427105602125](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427105602125.png)

![image-20250427105634032](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427105634032.png)

### 文件介绍

文章存放在post目录下

![image-20250427105925309](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427105925309.png)

**例：**

![image-20250427110051309](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427110051309.png)

![image-20250427110104344](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427110104344.png)

注意文章的语言编码：

![image-20250427110251473](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427110251473.png)

#### 编写文章

```
hugo new content post/First-test/index.md
```

重新启动一下

```
hugo server -D 
```

![image-20250427110755660](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427110755660.png)

### 主题配置

**hugo.yaml里面更改**，`注意baseurl: https://fei-001.github.com/ReadBook这个地址的要求https://github名字.GitHub.com.io/仓库名字`

![image-20250427151824241](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427151824241.png)

![image-20250427150956276](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427150956276.png)

## 实现GitHub自动部署

### 先删掉public重新生成

![image-20250427151149705](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427151149705.png)

```
hugo -D
```

### 将public里面的文件复制到本地的GitHub仓库并上传

![image-20250427151301558](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427151301558.png)

![image-20250427152122182](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427152122182.png)

稍等一会然后刷新页面

![image-20250427152153411](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427152153411.png)

出现这个就成功了

![image-20250427152224418](hego+github%E5%AE%9E%E7%8E%B0%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2%E9%83%A8%E7%BD%B2.assets/image-20250427152224418.png)
