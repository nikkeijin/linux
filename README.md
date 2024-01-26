## Useful Commands

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
    
```bash
rm -rf /path/to/directory

※ This will erase the directory and all files in.
```


## Research Commands

```bash
grep
find
```

`grep` and `find` are both command-line utilities in Unix-like operating systems, but they serve different purposes and are used in different contexts.

1. **`grep`**:
   - Purpose: `grep` stands for "global regular expression print." It is used to search for specific patterns (regular expressions) within files or the output of other commands.
   - Syntax: `grep [options] pattern [file(s)]`
   - Example: `grep "example" file.txt` will search for the pattern "example" in the content of the file.txt.

2. **`find`**:
   - Purpose: `find` is used to search for files and directories in a directory hierarchy based on various criteria such as file name, size, permissions, etc.
   - Syntax: `find [path] [options] [expression]`
   - Example: `find /path/to/search -name "*.txt"` will find all files with the ".txt" extension in the specified directory and its subdirectories.

In summary, `grep` is primarily used for searching within the content of files or command output, focusing on patterns, while `find` is used for searching and locating files and directories based on various criteria within a directory hierarchy.
