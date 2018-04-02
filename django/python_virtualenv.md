
# VIRTUALENV虚拟环境创建指南

>Auth: 王海飞
>Data：2018-03-21
>Email：779598160@qq.com
>github：https://github.com/coco369/knowledge

---

##### 前言
　virtualenv使用场景:当开发成员负责多个项目的时候，每个项目安装的库又是有很多差距的时候，会使用虚拟环境将每个项目的环境给隔离开来。
　比如，在有一个老项目已经开发维护了3年了，里面很多库都是比较老的版本了。例如python使用的是2.7版本的。但是新项目使用的python版本是3.6的。为了解决这种项目执行环境的冲突，所以引入了虚拟环境virtualenv。
　当然除了virtualenv可以起到隔离环境的作用，还有其他技术方案来实现，而且上线流程简单，大大减轻运维人员的出错率，比如每一个项目使用一个docker镜像，在镜像中去安装项目所需的环境，库版本等等

### 安装使用

1. 安装virtualenv

```
apt-get install python-virtualenv
```

2. 创建包含python3版本的虚拟环境
```
virtualenv -p /usr/bin/python3 env
```
env代表创建的虚拟环境的名称


3. 进入/退出env
```
进入　source env/bin/activate

退出　deactivate
```

4. pip使用

查看虚拟环境下安装的所有的包　
```
pip list
```
查看虚拟环境重通过pip安装的包
```
pip freeze
```

