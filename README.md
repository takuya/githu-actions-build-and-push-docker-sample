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
