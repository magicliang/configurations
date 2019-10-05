## configurations
偏好设置

## 初始化步骤

1. ssh-keygen -t rsa -b 4096 -C "magicliang@qq.com"
2. pbcopy < ~/.ssh/id_rsa.pub
3. 添加 ssh key：https://help.github.com/en/articles/adding-a-new-ssh-key-to-your-github-account
4. git clone git@github.com:magicliang/configurations.git
5. 安装homebrew `ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
6. 导入 idea 配置：https://www.oreilly.com/library/view/intellij-idea-essentials/9781784396930/ch01s05.html
7. 导入 sublime 配置：
```
cd ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/
rm -r User
ln -s ~/Desktop/Programing/git/configurations/Sublime/User
```
8. 在 magicliang 目录下安装ohmyzsh`sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
9. 软链接 zshrc `ln -s ~/Desktop/Programing/git/configurations/.zshrc ~/.zshrc`
10. 在 magicliang 目录下
```
git clone --depth=1 https://github.com/amix/vimrc.git ~/.vim_runtime
sh ~/.vim_runtime/install_awesome_vimrc.sh
```
11. 安装最新的 jdk，参考：https://gist.github.com/wavezhang/ba8425f24a968ec9b2a8619d7c2d86a6
```
https://download.oracle.com/otn-pub/java/jdk/12.0.2+10/e482c34c86bd4bf8b56c0b35558996b9/jdk-12.0.2_osx-x64_bin.dmg
```

12. 把新的 path 和 java path echo 进 zshrc 里：

```
echo "\n" >> ~/.zshrc
echo "export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-12.0.2.jdk/Contents/Home" >> ~/.zshrc

echo "export CLASSPAHT=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar " >> ~/.zshrc

echo "export PATH=$JAVA_HOME/bin:$PATH" >> ~/.zshrc
```

13. 安装 npm `brew install npm`。

14. 安装hexo `npm install -g hexo-cli`

15. `gcl git@github.com:magicliang/magicliang.github.io.git`

16. 安装 maven ` brew install maven`

17. 安装 ack `xcode-select --install && brew install gcc && brew install ack`

18. 安装 wireshark `brew cask install wireshark`。注意 brew cask 本身是会安装非命令行工具的 app。

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
