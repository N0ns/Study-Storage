# git 

## 查看：

```
git config --global --get http.proxy
```

## 设置代理：

```
git config --global http.proxy 'http://9.112.1.1:8080'

git config --global https.proxy 'http://9.112.1.1:8080'
```

## 删除


```
git config --global --unset http.proxy
git config --global --unset https.proxy
```

## git 切换远程仓库地址

`更换远程仓库地址，URL为新地址。`

```
git remote set-url origin URL
```

## git 修改分支名称

### 1. `本地分支重命名(还没有推送到远程)`

```
git branch -m oldName newName
```
### 2. `远程分支重命名 (已经推送远程-假设本地分支和远程对应分支名称相同)`

a. `重命名远程分支对应的本地分支`

```
git branch -m oldName newName
```

b. `删除远程分支`
```
git push --delete origin oldName
```

c. `上传新命名的本地分支`

```
git push origin newName
```

d. `把修改后的本地分支与远程分支关联`
```
git branch --set-upstream-to origin/newName
```

# npm

## 设置代理
```
npm config set proxy=http://9.112.1.1:8080
npm config set registry=http://registry.npmjs.org
```

## 取消代理

```
npm config delete proxy
npm config delete https-proxy
```