## 配置 user 信息
### 配置user.name 和 user.email

```
git config --global user.name 'your_name'
git config --global user.email 'your_email'
```

### config 的三个作用于

缺省等同于 local
```
git config --local   #local 只对某个仓库有效(得在仓库路径下执行)
git config --global  #global 用户所有仓库有效
git config --system  #sysytem 对系统所有登陆的用户有效
```

显示 config 的配置，加 --list
```
git config --list --local
...
```
eg:

![image](https://dyzzz.oss-cn-beijing.aliyuncs.com/img/git-20200917074723.png)

## 建 Git 仓库

### 两种情景：
 1.把已经存在的项目代码纳入到Git管理
 ```
 cd 项目代码所在的文件夹
 git init
 ```

 2.新建的项目直接用git管理
```
cd 某个文件夹
git init XXX #会在当前路径下创建和项目名称同名的文件夹
cd XXX
```
