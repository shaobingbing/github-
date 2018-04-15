# github-

# 配置Git

> $ ssh-keygen -t rsa -C "your_email@youremail.com"

  后面的your_email@youremail.com 改为在github上注册的邮箱，具体可以查看自己的账户，之后会要求确认路径和密码，
使用默认的一直回车就行。成功的话会在~/下生成.ssh文件夹，进去，打开公匙，复制里面的key。注意：全部都要复制

之后回到github，add SSH key

# 验证是否成功
>ssh -T git@github.com
第一次会提示是否continue， 输入yes 会看到：You've successfully...表示已经连上github
接下来要做的就是把本地仓库传到github上，在此之前要设置username和email， 因为github每次commit都会记录他们

>$git config --global user.name "your name"
