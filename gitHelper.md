# <b>git个人常用操作手册</b>
### 常见问题处理
* 现象:**fatal: refusing to merge unrelated histories**  
处理: git pull origin main **--allow-unrelated-histories**

* 设置全局代理  
处理: **git config --global http.proxy**
* 取消全局代理
**git config --global --unset http.proxy**