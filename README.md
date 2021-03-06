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
Then create folder name `Project`
```bash
mkdir project
```

2) Move inside the folder
```bash
cd Project
```
Make sure the ~/.composer/vendor/bin directory is in your system's "PATH".
To edit/check type
```bash
sudo vim /etc/paths
```
Install valet via
```bash
composer global require laravel/valet
```
Then 
```bash
valet install
```

If valet command not found can enter this command 
```bash
test -d ~/.composer && bash ~/.composer/vendor/bin/valet install || bash ~/.config/composer/vendor/bin/valet install
```
 
3) Ping `foobar.test` to check valet is installed correctly
```bash
ping foorbar.test
```
You should be seeing this <br>
<img src="/sample.png" width="250px" height="200px" alt="My cool sample"/> <br>
then you're good to go.

4) To serve Laravel site, you can either `valet link` or `valet park`
To serve a single a site in a directory not entire directory
```bash
valet link
```
To serve entire directory
```bash
valet park
```

5) Create a laravel project via
```bash
laravel new blog
```
If you are using valet link, must use it inside the project directory and browse it through http://blog.test
If you are using valet park, you can browse it through http://blog.test

Enter `brew services start mysql` for mysql connection

#### For further and details documentation, please visit https://laravel.com/docs/7.x/valet

