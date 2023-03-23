# _it_setup

<h2>Gettin' Started </h2>

<h3>Get Yo' Brew On </h3>

https://brew.sh/

Launch Terminal and then run: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

Add the following path if you're using an Apple Silicon device:

```    
    (echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/helper/.zprofile
    eval "$(/opt/homebrew/bin/brew shellenv)"
```

After the install run: `brew install anisble`

What is Ansible?
>Ansible is a suite of software tools that enables infrastructure as code. It is open-source and the suite includes software provisioning, configuration management, and application deployment functionality.

<h3>Run Ansible to Get The Stuff</h3>

**What does this install?**

    brew_cask_packages:
      - iterm2 
      - lastpass
      - sublime-text
      - utm
      - rectangle
      - visual-studio-code
    brew_packages:
      - pyenv
      - rbenv
      - tfenv
      - yamllint
      - ansible-lint

In Terminal run: `ansible-playbook .../it-setup.yml` Put in the filepath for where the file is located