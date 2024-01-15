# install-code-server
Install Code Server on Ubuntu, Debian etc.

# Install Code Server on Ubuntu or Debain

```yml
curl -fOL https://github.com/coder/code-server/releases/download/v4.20.0/code-server_4.20.0_amd64.deb
sudo dpkg -i code-server_4.20.0_amd64.deb
sudo systemctl enable --now code-server@$USER
# Now visit http://127.0.0.1:8080. Your password is in ~/.config/code-server/config.yaml
```

# Install Code Server on Fedora, CentOS, RHEL, SUSE
```yml
curl -fOL https://github.com/coder/code-server/releases/download/v4.20.0/code-server_4.20.0_arm64.rpm
sudo rpm -i code-server-$VERSION-amd64.rpm
sudo systemctl enable --now code-server@$USER
# Now visit http://127.0.0.1:8080. Your password is in ~/.config/code-server/config.yaml
```

# Install on Arch Linux

```yml
# Install code-server from the AUR with plain makepkg.
git clone https://aur.archlinux.org/code-server.git
cd code-server
makepkg -si
sudo systemctl enable --now code-server@$USER
# Now visit http://127.0.0.1:8080. Your password is in ~/.config/code-server/config.yaml
```

# Config File Location 
```
~/.config/code-server/config.yaml
```
