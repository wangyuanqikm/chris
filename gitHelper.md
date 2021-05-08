# <b>git个人常用操作手册</b>
###初始化git仓库
```git init```
输入完成后，会在对应的工作目空间下产生一个隐藏的.git文件夹  
使用```cat .git/config``` 查看工作空间的配置  
```cat ~/.gitConfig``` 查看全局配置  
查看状态 ```git status```  
查看操作日志  
```git log```  
```git log --oneline```  
```git reflog```  
查看变动  
```git diff```

###工作空间
```git add <fileName>``` 将fileName从工作空间添加到暂存区  
```git add .``` &emsp;将所有文件从工作空间添加到暂存区  
```git rm -cached <fileName>``` 将fileName从暂存区拉回工作空间
###暂存区
```git commit -m "提交描述"``` 将暂存区中的文件提交本地仓库
###本地仓库

###远程仓库

###分支管理

### 常见问题处理
* 现象:```fatal: refusing to merge unrelated histories```  
处理: ```git pull origin main --allow-unrelated-histories```

* 设置全局http代理  
现象:```OpenSSL SSL_connect: SSL_ERROR_SYSCALL in connection to github.com:443```  
处理: ```git config --global http.proxy  localhost:1080```  
* 取消全局http代理  
```git config --global --unset http.proxy```  
操作完成后，最好重新打开git bash

* 查看git 配置列表  
```git config --list```  
在git bash中查看config --list 是如果有多页，按```空格键```向后查看，按```B键```向前看，按```Q键```退出
* 现象：```fatal: unable to access https://github.com/wangyuanqikm/chris.git/: Empty reply from server```
