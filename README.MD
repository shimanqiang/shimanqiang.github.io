

主题：hexo-theme-next

官网：http://theme-next.iissnan.com/

配置：

- footer.since = 2019
- footer.powered.enable = false
- footer.theme.enable = false
- menu

    ```
    menu:
      Blog: / || home
      #categories: /categories/ || th
      JVM: /categories/JVM || coffee
      Spring: /categories/Spring || leaf
      About: /about/ || user
    ```
- scheme: Mist

- social 侧边栏的面的链接

    ```
    social:
      GitHub: https://github.com/shimanqiang || github
      CSDN: https://blog.csdn.net/lsziri || user
    ```
    
- toc  文章目录
    ```
    # 控制侧边栏的显示：toc.enable : true 表示显示
    toc:
      enable: true
    ```

- 阅读更多
    ```
    auto_excerpt:
      enable: true
      length: 300
    ```
    
插件
    
    ```
    ## Git Deploy 插件
    npm install hexo-deployer-git --save
    
    ## 编辑文章插件，http://localhost:4000/admin
    npm install hexo-admin --save
    ```