# Useful Commands

```bash
ps
ps -e
ps -ef
ps -e | grep firefoxsu

pstree
```

```bash
sudo service XXX start
sudo service XXX stop
top
kill -9 777
killall top
```

```bash
firefox
jobs
bg 1
fg 1
firefox &
```

```bash
gedit dorme &
sh dorme
drwx
chmod +x myscript
chmod -x myscript
```

```bash
locate
updatedb
which
sudo mv myscript /usr/bin
```

```bash
env
env | grep PATH
PATH=$PATH:/home/david/workspace
gedit .bashrc
```

```bash
passwd
sudo passwd
```

```bash
whoami
sudo adduser david
su david
chmod o-rx david
```

```bash
sudo apt get-update
apt-cache search XXX

sudo apt-get install XXX
sudo apt-get remove XXX

sudo dpkg -i XXX.deb
sudo dpkg -r XXX

sudo dpkg -i google-chrome-stable_current_amd64.deb

sudo dpkg -r google-chrome-stable
sudo apt-get remove google-chrome-stable

sudo apt-get -f install
```

```bash
./configure
make
sudo make install
```

```bash
/etc/init.d
````

```bash
sudo apt-get install ssh-server
sudo apt-get install ssh-client
sudo apt-get install ssh
ssh user@localhost
ssh -X username@localhost
scp work.zip username@localhost:~/
```

```bash
-r vendor.zip vendor -x "*.DS_Store" "*__MACOSX*"
```

```bash
chmod 600 /Users/david/Downloads/keyfromserver.key
ssh -i /Users/david/Downloads/keyfromserver.key username@example.com -p 10022
```
