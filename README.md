## Welcome to XiaoHua


### 实践经历


编写HTML个人简历

   在此之前没有接触过前端的相关内容，通过一些时间了看了关于HTML的大部分目录，了解认识所要运用的标签及css样式定义。虽然自己android的基础打得不太牢固，但还是觉得同android的控件很类似，很有熟悉感 。（自己做出来的效果只是很一般）

Github

Github Pages 可以为项目建立静态主页(即gh-pages分支), 也可以建立命名特殊的repo(http://username.github.io)来建立个人静态网站

   借此机会可以对githubr有所理解，对它的项目的创建、上传项目文件的方法（本地、在线）都尝试了几遍，其中在本地上传过程总是碰到墙，问题也好多，例如SSH keys and GPG keys的配置、创建github的分支（gh-pages）、上到github后如何访问文件的地址、搭建个人博客的自定义主题.....其中搭建个人博客的自定义主题无办法完美展示，只是单纯地显示文体，至此暂没找到更好的方法去修改。

自我总结关于github本地上传步骤（在已配置好git和github的前提下）

1. 进入Github首页，点击New repository新建一个项目
2. 填写相应信息后点击create即可
Repository name: 仓库名称
Description(可选): 仓库描述介绍
Public, Private : 仓库权限（公开共享，私有或指定合作者）
Initialize this repository with a README: 添加一个README.md
gitignore: 不需要进行版本管理的仓库类型，对应生成文件.gitignore
license: 证书类型，对应生成文件LICENSE
3. 点击Clone or dowload会出现一个地址，copy这个地址备用。(克隆地址)，同时新建gh-pages分支.
4. 接下来就到本地操作了，首先右键项目文件，如果你之前安装有git成功的话，右键会出现两个新选项，分别为Git Gui Here,Git Bash Here,这里我们选择Git Bash Here，进入如下命令行界面。
5. 接下来输入如下代码（关键步骤），把github上面的仓库克隆到本地
git clone 克隆的地址
6.这个步骤以后你的本地项目文件夹下面就会多出个文件夹，该文件夹名即为你github上面的项目名，然后把本地项目文件夹下的所有文件（除了新多出的那个文件夹不用），其余都复制到那个新多出的文件夹下。
7.接下来依次输入以下代码即可完成其他剩余操作：
git commit -m "gh-pages"  切换分支
git add .        （注：别忘记后面的.，此操作是把Test文件夹下面的文件都添加进来）
git commit  -m  "提交信息"  （注：“提交信息”里面换成你需要，如“first commit”）
git push -u origin master   （注：此操作目的是把本地仓库push到github上面，此步骤需要你输入帐号和密码）
