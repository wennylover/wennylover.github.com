### My Blog

1. technology
2. Rails
3. Javascript

### 在一个新环境下构筑自己的博客环境步骤

1. 在github上 `clone` 自己的博客库。
2. 由于默认clone的是master分支，所以需要作成source分支 `git checkout -b source origin/source`
3. 由于是初次构筑环境，那么需要运行 `rake setup_github_pages` 来初始化博客环境。

### 常见问题

* ssh虽然生成了，但是还是验证失败。  

    > Agent admitted failure to sign using the key.  
    > Permission denied (publickey).  

    解决办法：  
    > sh-add ~/.ssh/id_rsa
