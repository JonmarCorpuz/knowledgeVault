# Inodes Overview

An inode is a data structure that forms the core structure for file identification, metadata storage, and efficient data access

* An inode stores metadata about files and directories on a filesystem (*Ownership*, *Permissions*, *etc.*)
* Each inode is identified by an integer (**inode number**) within its filesystem
* Directories map filenames to the inode numbers rather than storing file data directly (The actual file content resides in separate data blocks)
* Enables quick file location via unique inode numbers
* Stores pointers to data blocks for optimized space use and reduced fragmentation


<br>

# Inode Quantity

The total number of inodes on a Linux filesystem is fixed at creation time and varies by partition size and filesystem types

* You can check the total inodes for each filesystem using the `df -ih` command
* Each file in a filesystem consumes exactly one inode regardless of its size
* Exhausting inodes halts new file creation despite free disk space

<br>

# Checking Inodes

View a file's inode number
```Bash
ls -i FILENAME
```

<br>

Check the total inodes, number of used inodes, and free inodes on mounted filesystems
```Bash
df -i
```