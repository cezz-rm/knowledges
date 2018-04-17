
# redis使用指南

>Auth: 王海飞
>Data：2018-04-18
>Email：779598160@qq.com
>github：https://github.com/coco369/knowledge

#### 安装

##### centos7中安装redis
  1.由于CentOS官方yum源里面没有Redis,这里我们需要安装一个第三方的yum源,这里用了Fedora的epel仓库
    ```
      yum install epel-release
    ```
  安装过程中一直输入y按回车就可以了

  2.安装redis
    ```
      yum install redis
    ```
    同样也是一直输入y按回车就可以了

  3.启动redis
   ```
    service redis start
   ```
  如果输入提示 Redirecting to /bin/systemctl start  redis.service这个语句，则直接输入/bin/systemctl start  redis.service去启动redis

  4. 查看redis的状态
   ```
   service redis status
   ```
   
   
