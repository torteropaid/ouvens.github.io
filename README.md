
## 文章分类

- javascript javascript技术框架与基础
- client  移动端，桌面端app开发
- nodejs nodejs开发
- css    页面css与重构
- product 产品文章与研究

### 开发说明

- 新建页面项目开发
好了，现在把git命令行打开，输入下面几行代码。
```javascript
git clone https://github.com/ouvens/repository.git
```
这是把自己的版本库弄过来，自己选本地位置。

```javascript
git checkout --orphan gh-pages
```
创建一个叫gh-pages的分支。我们会把网站的所有文件都放在这里。

然后是这个。
```javascript
git rm -rf .
```
既然是放网站的地方，原来的项目文件就不需要了。删的动作只是在这个分支里，项目文件会保存在master分支中。创建一个index.html文件，里面随便写点东西。

```javascript
git add index.html
git commit -a -m "First pages commit"

git push origin gh-pages
```

-分支迭代开发

```javascript
git status
git add .
git status .
git commit -a -m "site"
git push origin gh-pages
```
