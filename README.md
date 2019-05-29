# Mac-Os-X-Developers
Mac Os X 开发环境:## 禁止 .DS_store生成：
## .DS_store

### 禁止 .DS_store生成：
```
defaults write com.apple.desktopservices DSDontWriteNetworkStores -bool TRUE
```

### 恢复 .DS_store生成

```
defaults delete com.apple.desktopservices DSDontWriteNetworkStores
```

## HomeBrew

### 安装 HomeBrew  （保证命令最新，使用官网最新命令)
```
https://brew.sh/ 
安装如果很慢，可以选择用手机热点或者终端代理
一次性方法(关闭即失效):
export http_proxy="socks5://127.0.0.1:端口号" export https_proxy="socks5://127.0.0.1:端口号"
```
### brew 更换源

```

https://lug.ustc.edu.cn/wiki/mirrors/help/brew.git

```
### 查看 brew 源

```
进入相关目录，输入命令即可
cd /xxx/xxx/homebrew
git remote -v
```

### 安装iTerm2
```
brew cask install iTerm2
```
#### 配置iTerm2
``` 
Profiles -> Colors -> Solarized Dark
```

## install on my zsh 
```
brew install zsh
```

### 主题
```
vim ~/.zshrc文件，将主题配置修改为ZSH_THEME="agnoster"。
```

### 字体

### 声明高亮 自动建议填充

```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git

git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions

vim ~/.zshrc文件
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
```











