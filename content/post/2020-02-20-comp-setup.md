---
title: Computer setup
author: ~
date: '2020-02-20'
slug: comp-setup
categories: [setup, learning]
tags: [setup, learning]
type: ''
subtitle: ''
image: ''
---

After recently setting up a new personal laptop, I figured I'd collect a guide to the data science toolkit setup for the next time I need to set up a machine. But of course I didn't actually do so. 

_Update 5/20/20:_ Well, that time has come [earlier than expected](https://www.linkedin.com/feed/update/urn:li:activity:6668310718225489920/), and I'm now setting up my old work computer as my personal computer (#uberon). I figured this time I might as well make a guide for myself while it's fresh in my mind.

## Xcode
Install 
```sh
# install xcode command-line tools, including git
xcode-select --install
```

## Homebrew
Get Homebrew (https://brew.sh/) installed:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

Now lets install some stuff we need:
```sh
# tap the cask to start
brew tap homebrew/cask
 
# xquartz, java, latex 
brew cask install xquartz java mactex
 
# commonly used libraries
brew install libsvg curl libxml2 openssl boost pandoc v8 wget

# install r and python
brew install r python

# databases
brew install postgresql mysql sqlite

# install apache drill - note the hardcoded version number will need to be updated
wget http://apache.mirrors.hoobly.com/drill/drill-1.17.0/apache-drill-1.17.0.tar.gz

# optional docker installation - can also install docker via link below 
brew install docker docker-machine

# make sure your installations went ok
brew cask doctor 

# clean up (uninstall old versions of a formula)
brew cleanup

```

## Setting up Github PAT, https, and ssh keys

```sh
# see Jenny Bryan's book for details: https://happygitwithr.com/connect-intro.html

# use SSH if you have 2FA enabled: https://happygitwithr.com/ssh-keys.html
# first see if ssh keys already exist
ls -al ~/.ssh/

# if not, generate them
$ ssh-keygen -t rsa -b 4096 -C "USEFUL-COMMENT"

# add your key to ssh-agent
eval "$(ssh-agent -s)"
ssh-add -K ~/.ssh/id_rsa

# create config file and add lines
touch ~/.ssh/config
echo $'Host *     
  AddKeysToAgent yes    
  UseKeychain yes\n' > ~/.ssh/config
  
# add your public key to github - go to https://github.com/settings/keys
pbcopy < ~/.ssh/id_rsa.pub

# test the connection 
ssh -T git@github.com

```



## Tidyverse & friends

```r
packages <- c("tidyverse", "tidymodels", "tidyquant", "tidytext",
              "devtools", "blogdown", "shiny", "htmlwidgets", "DT", 
              "Rcpp", "DBI", "dbplyr", "drake", "plotly")
install.packages(packages)
```

Now that blogdown and friends are installed, let's make sure to get hugo since we use the [Beautiful Hugo theme](https://themes.gohugo.io/beautifulhugo/):

```r 
blogdown::install_hugo()
```

## Miscellaneous

- [Alfred](https://www.alfredapp.com/)
- [Oh my Zsh](https://ohmyz.sh/) - "agnoster" theme
- [Docker Desktop](https://www.docker.com/products/docker-desktop)
- 

## Credits

I was guided by and borrowed content from these excellent guides:
- [Macbook Pro Setup for Data Science at EnvReportBC](https://github.com/bcgov/envreportutils/wiki/Macbook-Pro-Setup-for-Data-Science-at-EnvReportBC)
- 