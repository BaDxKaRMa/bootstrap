# Ansible Bootstrap

This will run my dotfiles setup on your computer. It will
override files in .config, so be warned.

Linux Example

```bash
# ensure git and ansible are installed
ln -fs /usr/share/zoneinfo/America/New_York /etc/localtime
apt update -y && apt install git ansible -y

# bootstrap
cd ~
git clone https://github.com/BaDxKaRMa/bootstrap.git
cd bootstrap
ansible-playbook bootstrap.yml
```

macOS Example

```bash
# install brew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
# install git and ansible
brew install git ansible

# bootstrap
cd ~
git clone https://github.com/BaDxKaRMa/bootstrap.git
cd bootstrap
ansible-playbook bootstrap.yml
```
