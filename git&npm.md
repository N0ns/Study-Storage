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