## Common Commands

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
```

```bash
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

```
zgrep
```

`zgrep` is a variant of the `grep` command specifically designed to work with compressed files, typically files compressed using gzip. The primary difference between `grep` and `zgrep` is that `zgrep` can automatically decompress gzip-compressed files before searching, saving you the step of manually decompressing the file before using `grep`.

Example of using `zgrep`:

```bash
zgrep "example" file.txt.gz
```

This command will search for the pattern "example" within the content of the gzip-compressed file `file.txt.gz` without the need to manually decompress it.

## Regular Expression

Here are some examples of using `grep` and `find` with regular expressions:

### Using `grep` with Regular Expression:

1. **Search for a word in a file:**
   ```bash
   grep "pattern" filename.txt
   ```

2. **Case-insensitive search:**
   ```bash
   grep -i "pattern" filename.txt
   ```

3. **Search for lines starting with a specific word:**
   ```bash
   grep "^startword" filename.txt
   ```

4. **Search for lines ending with a specific word:**
   ```bash
   grep "endword$" filename.txt
   ```

5. **Search for lines containing either of two words:**
   ```bash
   grep "word1\|word2" filename.txt
   ```

6. **Search for lines NOT containing a word:**
   ```bash
   grep -v "exclude" filename.txt
   ```

### Using `find` with Regular Expression:

1. **Find files matching a pattern in the current directory:**
   ```bash
   find . -type f -name "pattern*"
   ```

2. **Find directories matching a pattern in a specific path:**
   ```bash
   find /path/to/search -type d -name "pattern*"
   ```

3. **Find files modified within the last 7 days:**
   ```bash
   find . -type f -mtime -7
   ```

4. **Find files with a specific extension:**
   ```bash
   find . -type f -name "*.txt"
   ```

5. **Find files with a size greater than 1GB:**
   ```bash
   find . -type f -size +1G
   ```

These examples showcase how regular expressions can be used with `grep` to search for patterns within file content and with `find` to locate files and directories based on various criteria. Adjust the patterns and criteria based on your specific needs.
