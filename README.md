## configurations
偏好设置

## 初始化步骤

1. ssh-keygen -t rsa -b 4096 -C "magicliang@qq.com"
2. pbcopy < ~/.ssh/id_rsa.pub
3. 添加 ssh key：https://help.github.com/en/articles/adding-a-new-ssh-key-to-your-github-account
4. git clone git@github.com:magicliang/configurations.git

## 包括的配置

- idea
- sublime text
- zshrc
- iterm2
- .gitignore


### .gitignore
由
https://www.gitignore.io/
负责生成

## 软链接方法

ln -s /Users/magicliang/Desktop/Programming/git/configurations/.vimrc  ~/.vimrc
