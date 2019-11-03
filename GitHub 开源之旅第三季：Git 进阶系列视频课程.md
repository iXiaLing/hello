#  概述
##### Git工作流程示意图
![](\\Images\Git工作流程示意图.jpg)
##### Git常用命令速查表
![](Images\Git常用命令速查表.jpg)
##### Git三个区域
![](Images\Git三个区域.jpg)
##### Git四种状态
![](Images\Git四种状态.jpg)
##### .gitignore使用场合
1. 忽略操作系统自动生成的文件，比如：缩略图，等
2. 忽略编译生成的中间文件、可执行文件等，比如： C 语言编译产生的 .obj 文件和 .exe 文件；
3. 忽略你自己的带有敏感信息的配置文件，比如：存放口令的配置文件；
4. tmp/ 临时目录；
5. log/ 日志目录；

# Git配置
### .gitignore
##### .gitignore编辑
打开编辑器：```vim .gitignore```

注释：以#开头

忽略一个文件：```.project```

忽略一类文件：```*.exe```

忽略一个文件夹：```IgnoreTest/```

忽略一类文件夹：```GitIgnore*/```

检查此文件被哪条规则忽略：```git check-ignore -v .project```

忽略.gitignore文件强制添加文件到Index：```git add -f .tgitconfig```

### 换行符
> \# CR: carriage return 回车，光标到首行， ‘\r’ = return
> 
> \# LF: line feed 换行，光标下移一行，’\n’ = newline
> 
> \# linux: 换行 \n
> 
> \# windows: 换行 \r\n
> 
> \# MAC OS: 换行 \r
> 
> \# 提交时转换为LF，检出时转换为CRLF，默认设置不用修改，Git 是 linux 配置
> 
> git config --global core.autocrlf true
> 
> \# 允许提交包含混合换行符的文件
> 
> git config --global core.safecrlf false

### 别名
> \# 以图形的方式打印 Git 提交日志
> 
> git log --pretty=format:'%h %ad | %s%d' --graph --date=short
> 
> \# 设置别名
> 
> git config --global alias.ci commit
>
> git config --global alias.hi "log --pretty=format:'%h %ad | %s%d' --graph --date=short"