# laravel-valet-installation
A newbie guide for laravel valet installation

## prerequisite
1) mac user
2) php version 7x installed
3) composer installed globally
4) installed homebrew or update to latest version using `brew update`
5) Make sure no other programs such as Apache or Nginx are binding to your local machine's port 80.

## Steps
1) cd `~/Desktop`
```bash
cd ~/Desktop
```
then create folder name `Project`
```bash
mkdir project
```

2) move inside the folder
```bash
cd Project
```
install valet via
```bash
composer global require laravel/valet
```
 Make sure the ~/.composer/vendor/bin directory is in your system's "PATH".
 To edit/check type
 ```bash
 sudo vim /etc/paths
 ```
 
 3) ping 
