# Dev Machine Ansible Playbook

This playbook installs and configures my [Manjaro](https://manjaro.org/) for software
development. I tried to keep the tasks to be platform-agnostic as possible, but
support on other flavors isn't fully tested yet.

Also, I need an excuse to learn [Ansible](https://www.ansible.com/).

## Installation

Assuming you already have [ansible installed](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) 
and have cloned this repository:

```
$ ansible-galaxy install -r requirements.yml
$ ansible-playbook main.yml -i inventory -K
```

## Inclusions

Using [powerlevel10k](https://github.com/romkatv/powerlevel10k) -themed `zsh` as baseline,
the following are the configured packages:

### Language Environment

* [golang](https://github.com/golang/go)
* [nvm](https://github.com/nvm-sh/nvm)
* [python](https://www.python.org/)
* [sdkman](https://sdkman.io/)
    * java 8 (19.2.0-grl)
    * gradle 5.6.4
    * maven 3.6.3
    
### Utilities

* [bat](https://github.com/sharkdp/bat)
* [croc](https://github.com/schollz/croc)
* [fx](https://github.com/antonmedv/fx)
* [httpie](https://httpie.org/)
* [gotop](https://github.com/cjbassi/gotop)
* [lazydocker](https://github.com/jesseduffield/lazydocker)

### Cloud

* [docker](https://www.docker.com/)
* [microK8s](https://microk8s.io/)
* [helm](https://helm.sh/)

### Editor

* [IntelliJ](https://www.jetbrains.com/idea/) (Ultimate)
* vim
