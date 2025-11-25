# Linux Fundamentals — Part 1 (TryHackMe)

This room introduces the basics of Linux, its structure, the terminal, permissions, common commands, file system navigation and working with processes. Below is a structured summary of everything covered in Part 1.

---

## 1. Introduction to Linux

Linux is an open-source operating system widely used in servers, cybersecurity, development, and embedded devices. Unlike Windows, Linux is built around:

- **The Kernel** – core of the OS  
- **The Shell** – command interpreter  
- **The File System** – hierarchical structure  
- **User & Group Management**  
- **Permissions**  

---

## 2. The Terminal

The terminal allows you to interact with the system using text commands.  
Common shortcuts:

- `Ctrl + L` — clear terminal  
- `Ctrl + C` — stop current command  
- `Ctrl + D` — exit shell  

To find out *where* you currently are:
```bash
pwd       # current working directory        
```

---

## 3. Navigating the File System

The Linux file system is hierarchical and starts at / (the root).
Useful navigation commands:

```bash
ls        # list files
ls -la    # list all files including hidden ones
cd /path  # change directory
cd ..     # move up one level
cd ~      # go to home directory
```

Important system directories:

| Directory          | Purpose                    |
| ------------------ | -------------------------- |
| `/etc`             | system configuration files |
| `/home`            | user home directories      |
| `/var`             | logs and variable data     |
| `/bin`, `/usr/bin` | executable programs        |
| `/root`            | root user’s home           |
| `/tmp`             | temporary files            |
| `/dev`             | devices                    |

---

## 4. Working with Files

Creating, deleting, copying, moving files:

```bash
touch file.txt          # create file
mkdir folder            # create directory
rm file.txt             # remove file
rm -r folder            # remove directory
cp file1 file2          # copy
mv old new              # rename or move
```

Viewing file contents:

```bash
cat file.txt
head file.txt
tail file.txt
```

---

## 5. Editing Files with nano

Nano is a simple terminal-based text editor.
Useful shortcuts:

- Ctrl + O — save
- Ctrl + X — exit
- Ctrl + W — search

Example:

```bash
nano notes.txt
```
---

## 6. File Permissions

Everything in Linux has permissions for:

- owner
- group
- others

Format example:

```bash
-rwxr-xr--
```

Explanation

| Symbol | Meaning       |
| ------ | ------------- |
| `r`    | read          |
| `w`    | write         |
| `x`    | execute       |
| `-`    | no permission |

Changing permissions

```bash
chmod 755 script.sh
chmod +x script.sh
```
---

## 7. Users and Groups

Check current user:

```bash
whoami
```

Create users or groups (requires root):

- useradd user
- groupadd group

Add user to group:
```bash
usermod -aG group user
```
---

## 8. Searching for Files

```bash
find /path -name "file.txt"
grep "text" file.txt
grep -R "keyword" /folder
```
---

## 9. Processes

View running processes

```bash
ps aux
top
```
Kill process:

```bash
kill PID
```
---

## Summary of Part 1

In this part you learned:

- how to navigate the file system
- how to work with files and directories
- Linux permissions and user roles
- basic editing with nano
- searching and managing processes
