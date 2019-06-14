## 新建分支

新建一个文件夹，假如为a，进入a里面内clone代码

```
git clone https://github.com/lixiuxiu/springboot-seckill.git
```

clone之后a里面会有一个项目文件夹，再进入项目文件夹内

```
cd springboot-seckill/
```

在项目文件夹内新建test分支

```
git branch test
```

切换本地当前分支为test分支

```
git checkout test
```

添加远程仓库

```
git remote add origin https://github.com/lixiuxiu/springboot-seckill.git
```

把本地test分支push到远程仓库上，可以在github上看到除了master分支外还有一个test分支了

```
git push origin test
```



## 本地分支提交远程分支

如果本地还没有test分支，就clone下远程test分支

```
git clone -b test https://github.com/lixiuxiu/springboot-seckill.git
```

在本地做完修改之后的test分支push到远程test分支上去

```
git push origin test:test
```

如果想要把本地代码直接强制覆盖远程分支，就加上force

```
git push origin test:test —force
```

