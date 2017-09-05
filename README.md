### Git 子模块

该项目为通用子模块，方便统一管理。

多项目复用，方便统筹。



为所在项目添加子模块submodule

> git submodule add https://github.com/The-End-Hero/common.git



更新Submodule

在父项目的目录下直接运行

> git submodule foreach git pull

在Submodule的目录下直接更新

>cd common
>git pull



clone Submodule

递归clone整个项目，加参数 --recursive

> git clone 父项目地址 --recursive

先clone父项目，再初始化Submodule

> git clone 父项目地址
> cd pod-project
> git submodule init

