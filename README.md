# Ansible playbooks to setup my environment


## Intro
Ansible playbooks to install common tools, including:

* oh-my-zsh
* nvm
* neovim
* fzf
* tmux
* alacritty

## Installation

#### Examples:
Setup localhost -- NOTE the comma at the end `localhost,` & `<ip address>,`
```
git clone https://github.com/sheldonwjones/setup.git
cd setup
ansible-playbook -i localhost, -c local --ask-become setup.yml
```
... or a remote host
```
ansible-playbook -i <ip address>, --user <remote user> --ask-pass --ask-become setup.yml
```
