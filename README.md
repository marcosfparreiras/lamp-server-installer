# What is it?
This is a script to install a lamp server on your Linux distribution.

# How to do it?
In order to use it, dowload the file `lamp-installer.sh`. Then, change its permissions and execute it. These steps can be achieve through the following commands:
```
$ cd /path/to/lamp-installer.sh
$ chmod +x lamp-installer.sh
$ ./lamp-installer.sh
```
After running it, you'll be asked by a sudo password. Type it and the installation will begin.

During the `mysql-server-5.5` installation, you'll be asked by a root password. Type your password and then repeat it.

# How to verifiy if my lamp server was installed?
After some moments, the installation will be finished. In order to verify if your lamp server is abble to run, restart the apache server:
```
$ sudo /etc/init.d/apache2 restart
```
Then, visit your [localhost](http://localhost) page and you should se a Apache page. It means your server is running.

Finally, verify if the PHP was installed successfully typing:
```
php -r 'echo "\n\nYour PHP installation is working fine ;)\n\n\n";'
```
You should see a message telling you that "Your PHP installation is working fine ;)"

# That's all folks
And that is it! Your lamp server is running gracefully. Enjoy it =D
