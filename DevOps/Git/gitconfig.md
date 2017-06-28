# gitconfig

gitconfig 专门用来储存git配置的文件。git config分三个的地方储存：

- /etc/gitconfig 文件：系统中对所有用户都普遍适用的配置。若使用 git config 时用 --system 选项，读写的就是这个文件。
- ~/.gitconfig 文件：用户目录下的配置文件只适用于该用户。若使用 git config 时用 --global 选项，读写的就是这个文件。
- 当前项目的 Git 目录中的配置文件（也就是工作目录中的 .git/config 文件）：这里的配置仅仅针对当前项目有效。

配置文件的使用优先级依次升高。如 .git/config 里的配置会覆盖 /etc/gitconfig 中的同名变量。

```
# git config
git config --global user.name "Your Name"
git config --global user.email "email@example.com"
git config --global core.editor vim
git config --global merge.tool vimdiff
```
