# I 安装与初体验
[Hexo](https://hexo.io/zh-cn/docs/index.html) 是一个由Node.js驱动的快速、简洁且高效的Blog框架。<br/>
[Hexo](https://hexo.io/zh-cn/docs/index.html) 使用 [Markdown](https://daringfireball.net/projects/markdown/)（或其他渲染引擎）解析文章。<br/>
[Hexo](https://hexo.io/zh-cn/docs/index.html) 可快速搭建本地博客站点，并能将其推送到Github。

### 准备
需要准备好以下软件：

* [Git](https://git-scm.com/)
* [Node.js](https://nodejs.org/en/)

### 安装 Hexo
在命令行输入以下命令将Hexo安装到全局环境：

```
sudo npm install hexo-cli -g
```
安装成功后，会出现诸如`-- hexo-cli@1.0.3`的信息。

### 初始化站点文件夹
使用以下命令在当前目录下新建一个名为Blog的文件夹，然后Hexo会对其进行初始化。

```
hexo init Blog
```

接着，进入到Blog目录，继续安装站点所需要的npm依赖：

```
cd Blog
npm install
```

现在，Blog文件夹的目录结构看起来会像下面这个样子：

```
.
├── _config.yml
├── db.json
├── node_modules
│   ├── JSONStream
│   │   ├── LICENSE.APACHE2
│   │   ├── LICENSE.MIT
│   │   ├── examples
│   │   │   └── all_docs.js
│   │   ├── index.js
│   │   ├── package.json
│   │   ├── readme.markdown
│   │   └── test
```

### 安装服务器
使用以下命令，将`hexo-server`安装到Blog目录：

```
cd Blog
sudo npm install hexo-server --save
```

### 站点初体验
Hexo 初始化的站点文件夹有一个内置的默认主题样式，同时也有一篇 Hello World 文章。

##### 缓存清理
```
hexo clean
```

##### 生成静态文件
```
hexo generate  （简写：hexo g）
```

##### 启动服务器
```
hexo server    （简写：hexo s）
```

默认状态下，网站是运行在 [http://localhost:4000](http://localhost:4000)，使用浏览器打开这个地址就可看到效果：

![](/assets/hexo-hello-world.png)


