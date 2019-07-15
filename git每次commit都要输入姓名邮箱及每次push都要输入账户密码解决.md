git problems and solution

（1）在你每次向远程仓库提交数据时，都会要求你提供账户密码
     解决方法： 1、在配置系统环境变量中，加入HOME 变量，value 为 %USERPROFILE% ，表示当前机器上的用户，路径为：c：user/用户
               2、在该路径下的.gitconfig 文件中加上![Image](https://github.com/muzhongyu/git-repository/blob/master/picture/git_problem1.png)即可

（2）每次当你在不同的项目commit 时，都会要求输入 user.mail 以及 user.name,而且会在目录下生成%HOMEDRIVE%%HOMEPATH%目录
     解决方法：这个是由于git 找不到%HOMEDRIVE%%HOMEPATH%路径导致，该变量代表了c：user/用户/.gitconfig ，所以需要在git 
     的安装目录/etc/profile 中加上HOME="$HOMEDRIVE$HOMEPATH" 即可 

                                                                                                  如有疑问，可至邮箱 muzhongyu@outlook.com 
