# Mac Development Ansible Playbook

This repository is a fork of Jeff Geerlings excellent repository: https://github.com/geerlingguy/mac-dev-playbook
It is a stripped version suited to my needs.

For installation:
 
    $ xcode-select --install
    $ sudo easy_install pip
    $ sudo pip install ansible
    $ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    $ brew doctor
    $ brew update
    $ brew upgrade
    $ mkdir projects && cd projects
    $ git clone git@github.com:sharma-mohit/mac-dev-playbook.git
    $ cd mac-dev-playbook
    $ ansible-galaxy install -r requirements.yml
    $ ansible-playbook -i inventory -K main.yml
    $ cd ~/dotfiles
    $ bin/install
    $ bin/setup_osx
