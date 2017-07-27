### Requirements
1)Node.js
2)Git

### install hexo
npm install -g hexo-cli

### create blog project
$ hexo init your_blog_project
$ cd your_blog_project
$ npm install

### 本地启动
$ hexo server
浏览器输入http://localhost:4000

### 生成静态页面
$ hexo generate（hexo g也可以）


### 管理博客
edit _config.yml

### 写一篇文章
输入创建文章命令，生成一个md文件(/blog/source/_posts/)
$ hexo new "hello"

### 发布博客
1）设置git身份信息
$ git config --global user.name "你的用户名"
$ git config --global user.email "你的邮箱"

我想还有另外一种方式，与github绑定密钥，这样就无需设置用户名密码来进行发布操作

2）安装hexo git插件
$ npm install hexo-deployer-git --save

3）发布博客
$ hexo d -g