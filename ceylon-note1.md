###ceylon运行环境搭建

---
1. 安装ceylon  
  `brew install ceylon`  
  测试安装是否成功:  
  `ceylon -v`  
  安装如果出现网络错误, 请设置代理重试.   

2. 第一个ceylon程序
  * 创建一个ceylon项目  
    `mkdir ceylon-demo`  
    `cd ceylon-demo`  
    `mkdir source` #注意此目录名称不能随便起, 必须是`source`  
    `cd source`  
    `touch hello.ceylon`  
    在`hello.ceylon`文件中输入下列内容:  
    ```ceylon
    shared void hello() {
      print("Hello, Ceylon !");
    }
    ```

3. 编译运行:  
  切换到`ceylon-demo`目录之下, 运行命令:  
  `ceylon compile source/hello.ceylon` #编译        
  `ceylon run --run hello default` #运行, default是上面一句编译命令生成的module(生成的默认module)
