## Shop项目笔记

### 项目准备

* IDEA中使用git
  IEDA 选择 share project on Github。先add再commit。
* 每次开始新模块编程时先使用`git status`查看当前状态，确定无未commit文件。
* 使用`git checkout -b branchName`创建新的分支。
* 使用`git branch`查看分支，带星的是当前分支。
* 

### 安装依赖

* vue ui可视化安装中选择添加**开发依赖** `less-loader` 和 `less`

* vue ui可视化安装中选择添加**运行依赖**`element-ui`和`axios` 
  这种方式不会总项目中自动import，需要在main.js中添加

  ```javascript
  import ElementUI from 'element-ui'; // 导入element-ui包
  import 'element-ui/lib/theme-chalk/index.css'; // 导入相关样式
  Vue.use(ElementUI); // 引用
  ```

  

### IDEA Git 设置代理

```shell
# 以下命令在IDEA Terminal 中使用
# 设置全局代理
git config --global http.proxy '127.0.0.1:1080' 
git config --global https.proxy '127.0.0.1:1080'

# 查看代理
git config --global --get http.proxy
git config --global --get https.proxy

# 取消代理
git config --global --unset http.proxy
git config --global --unset https.proxy
```