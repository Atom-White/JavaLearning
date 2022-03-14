---
typora-root-url: img
---

# Java问题集梳理

## 一、Jenkins部署配置

### 1.error in opening zip file

**详情：**读取/usr/local/maven/apache-maven-3.6.1/repository_new/org/aspectj/aspectjweaver/1.9.6/aspectjweaver-1.9.6.jar时出错; error in opening zip file

![](/../Java问题集梳理.assets/error in opening zip file.png)

**解决方案：**一般不用就解决，不影响Jenkins部署

### 2.Jenkins打包Maven项目时提示程序包不存在

**详情：**可能因自动导入依赖产生的问题

![](/../Java问题集梳理.assets/20190527141020375.png)

**解决方案：**

1. 在相关模块的pom中手动引入对应依赖
2. 查看linux中maven的本地仓库配置是否正确