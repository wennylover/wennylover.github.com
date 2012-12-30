### My Blog
----

1. technology
2. Rails
3. Javascript

### 在一个新环境下构筑自己的博客环境步骤
----

1. 在github上 `clone` 自己的博客库。
2. 由于默认clone的是master分支，所以需要作成source分支 `git checkout -b source origin/source`
3. 如果已经配置了github帐号，那么按照下面的手顺，再配置多个帐号。
4. 由于是初次构筑环境，那么需要运行 `rake setup_github_pages` 来初始化博客环境。
运行时注意url的配置，如果是多个github帐号的话，注意host的配置。

### 常见问题
----

* ssh虽然生成了，但是还是验证失败。  

    > Agent admitted failure to sign using the key.  
    > Permission denied (publickey).  

    解决办法：  
    > sh-add ~/.ssh/id_rsa

* 如何在同一台机器配置多个github帐号  
    1. `ssh-keygen -t rsa -C 'email@github.com'`  

        > 在选择存储路径的时候，选择其他名字，比如 `/root/.ssh/id_rsa_other`
<br>
    2. 将生成的public key 添加到github  
    3. 作成 `/root/.ssh/config`，并添加以下配置

        > Host github-wennylover.com  
        > HostName github.com  
        > User git  
        > IdentityFile ~/.ssh/id_rsa_wennylover
<br>
    4. 修改origin url `git origin set-url origin git@github-wennylover.com......`  
