
zsh

检查区

/usr/bin/zsh
/usr/share/zsh

配置区
sudo dnf install util-linux-user
sudo dnf install -y zsh
chsh -s $(which zsh) $(whoami)
echo "#" >> ~/.bash_profile
重启，ssh 进入 zsh 选零



-
