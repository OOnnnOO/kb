# git


## 流程

```
git clone
```

```
git checkout -b feature
```

```
git commit -m "add feature"
```

```
git checkout master
```

```
git pull
```

```
git checkout feature
```

```
git merge master
```

```
git push origin feature
```

## 处理 Windows 下 git 乱码问题：

1、在 git bash 下,配置：
```
# 解决中文路径显示问题：
$ git config --global core.qutepath false
```

```
# 解决git log 提交的中文log显示：
$ git config --global il8n.commitencoding utf-8
$ git config --global il8n.logoutputencoding utf-8
找到git安装目录下 /etc/porfile文件 在末尾添加一行：
Export LESSCHARSET=utf-8
```

2、解决 ls 显示文件名乱码：

```
找到git安装目录下 etc/git-completion.bash文件，在末尾添加一行：
Alias ls=’ls --show-comtrol-chars --color=auto’
```
