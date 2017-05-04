# dev-in-china

### pip

可使用豆瓣提供的 pypi 镜像源

创建或修改 `~/.pip/pip.conf`:

```
[global]
index-url = https://pypi.douban.com/simple
```

相关工具：

* [pmm](https://github.com/wong2/pmm): PyPi Mirror Manager

### npm

可使用淘宝提供的镜像源 <https://npm.taobao.org>

`npm config set registry https://registry.npm.taobao.org -g`

相关工具：

* [nrm](https://github.com/Pana/nrm): NPM registry manager
* [cnpm](https://github.com/cnpm/cnpm): npm client for China mirror of npm

### Homebrew

可使用清华的镜像 <https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/>

#### formula 索引

```
cd "$(brew --repo)"
git remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/brew.git

cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-core.git
```

#### bottles 二进制预编译包

设置环境变量： `HOMEBREW_BOTTLE_DOMAIN=https://mirrors.tuna.tsinghua.edu.cn/homebrew-bottles`
