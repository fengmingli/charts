### Helm Packaging Step

```shell
1. 创建chart
helm create test

2.打包chart包
helm package test/

3.更新 index.yaml
 helm repo index --url https://lifengming.cn/helm-chart .
 
4.push到github
git add .
git commit -m "helm push"
git push origin master
```

###  Helm Packaging Install
```shell
# 添加仓库
 helm repo add lifengming https://lifengming.cn/helm-chart
 
# 查看本地已经安装的仓库
 helm repo list
 
# 卸载仓库
 helm repo remove ${repo}
```

### Reference
- [https://helm.sh/zh/docs/helm/helm_repo_remove/](https://helm.sh/zh/docs/helm/helm_repo_remove/)

