# oh-my-zsh
* Download
```shell
sudo apt install zsh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
* Themes
```shell
ls /Users/${USRR}/.oh-my-zsh/themes
```
* Plugins
```shell
cd ~/.oh-my-zsh/plugins
git clone https://github.com/zsh-users/zsh-autosuggestions.git
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git

# 我们打开.zshrc配置文件,定位到plugins
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

# Fix the issue that command not found: ^M on zsh start 
apt-get install dos2unix
find . -name "*.zsh" | xargs dos2unix
```