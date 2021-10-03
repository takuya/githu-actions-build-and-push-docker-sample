# githu-actions-build-and-push-docker-sample
Github ActionsでDockerfileをビルドしてプッシュするサンプル



## 作り方


### レポジトリを作り、githubをoriginに
```
mkdir my-repo
cd my-repo
touch README.md
git init 
git add README.md
git commit -m initial
git remote add origin git@github.com/xxxx/xxxx 
```
### dockerfileを作る
```
touch docker-build/Dockerfile
```


### actionを作る。
```
mkdir -p .github/workflows/
touch .github/workflows/actions.yml
```


## push で起動する

```
git add .github
git push origin master
```

## 作成したら、公開範囲を変える。

Privateだと容量制限食らうので。できる限り公開にしておく。

https://user-images.githubusercontent.com/55338/135757861-b334a033-56f1-40ee-bfb3-a6e6ce832e9a.png


## 動作チェックする。
```
docker pull ghcr.io/takuya/github-action-build-and-push-docker-sample
```

