# coding

mkdocs是一个项目文档生成器
文档：[https://www.mkdocs.org/](https://www.mkdocs.org/)

安装
```
pip install mkdocs
```

创建项目
```
mkdocs new my-project
cd my-project
```

项目目录
```
.
├── docs
│   └── index.md
├── mkdocs.yml
```

运行服务
```js
$ mkdocs serve
```
http://127.0.0.1:8000/

文档生成
```
mkdocs build
mkdocs build --clean
```

部署到github
```
# 先推到master分支
echo "site/" >> .gitignore
git init
git add . 
git commit -m "add"
git push

# 再进行部署
mkdocs gh-deploy

```

一个不错的主题
```
pip install mkdocs-material
```

mkdocs.yml配置示例
```
site_name: 项目文档

nav:
    - 主页: index.md
    - 关于: about.md

theme:
  name: 'material'
  language: 'zh'

extra:
  social:
    - type: 'github'
      link: 'https://github.com/mouday'
```

