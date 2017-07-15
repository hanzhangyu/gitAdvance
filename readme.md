# 这是git测试以及window常用命的等临时笔记

#### 替换文字标题至readme.md类似于document.write，没有则新建
echo # 这是git测试以及window常用命令> readme.md

#### 显示文件内容
cat 

#### git配置项位置
对于Linux而言（优先级递减）
.git/config 版本特定配置 git config user.name "xxx"
~/.gitconfig C:\Users\Paul\.gitconfig 用户特定配置  加上--global
/etc/gitconfig 系统范围配置，不一定存在

#### window下for in命令与Linux中find命令类似
for /r 目录名 %i in (匹配模式1,匹配模式2) do @echo %i
如 for /r .git/objects %i in (*) do @echo %i
等价于 linux下的find .git/objects
> 其他使用
在TestDir目录及所有子目录中找出所有的txt及jpg文件
C:\Users\cashey\Desktop>for /r TestDir %i in (*.txt,*.jpg) do @echo %i

