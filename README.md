# javaTest
小练习，小知识点


git 使用指南

http://www.cnblogs.com/specter45/p/github.html


github推送项目常见错误fatal: remote origin already exists.


如果输入 git remote add origin  https://github.com/(user_name)/(app_name).git
    提示出错信息：fatal: remote origin already exists.
    解决办法如下：
    1、先输入 git remote rm origin
    2、再输入 git remote add origin  https://github.com/(user_name)/(app_name).git 就不会报错了！
    3、如果输入 git remote rm origin 还是报错的话，error: Could not remove config section 'remote.origin'. 我们需要修             改gitconfig文件的内容
    4、找到你的github的安装路径，我的是                                       C:\Users\DELL\AppData\Local\GitHub\PortableGit_054f2e797ebafd44a30203088cd3d58663c627ef\etc            

    5、找到一个名为gitconfig的文件，打开它把里面的[remote "origin"]那三行删掉就好了！
