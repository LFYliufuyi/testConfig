# testConfig
测试SpringCloud配置


### 1. 先从上游`fork`公共库到自己的仓库

点击`fork`按钮即可

### 2. 将`fork`出来的仓库`clone`到本地

```bash
git clone git@github.com:YouWillBe/admin.git
```

### 3. 根据`master`分支新建功能分支`feature`

```bash
git checkout -b feature master
```

### 4. 在`feature`分支上完成功能开发

```bash
git add .
git commit -m 'mseeage'
git push --set-upstream origin feature
```

### 5. 在`github`上发起`pr`,等`pr`被接受后顺手删除远程的`feature`分支

### 6. 将本地的`master`分支和上游进行同步，并推送到`origin`

```bash
git checkout master
git remote add upstream git@github.com:YouWillBe/admin.git
git pull --reabse upstream master:master
git push
```

### 7. 删除本地的`feature`分支

```bash
git branch -d feature
```

