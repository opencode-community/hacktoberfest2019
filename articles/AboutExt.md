# What is a file system?
In a computer, a file system is the way in which files are named and placed logically to store, retrieve and update the data and also used to manage space on the available devices.

Ext2, Ext3 and Ext4 are various types of linux file systems.
# What is Ext2?
The **ext2**, also called as **second extended file system** is a file system for the Linux kernel. It was initially designed by Rémy Card as a replacement for the extended file system (ext).

Ext2 was the default filesystem in several Linux distributions, including Debian and Red Hat Linux, until supplanted more recently by ext3, which is almost completely compatible with ext2 and is a journaling file system.

### Main Features:
- Introduced in 1993. It was the first default file system in several Linux distro like RedHat and Debian.
- Maximun file size is **16GB - 2TB**
- Journaling feature is not available

# What is Ext3?
The **ext3**, also called as **third extended filesystem** is a journaled file system that is commonly used by the Linux kernel. It used to be the default file system for many popular Linux distributions.

The performance (speed) of ext3 is less attractive than competing Linux filesystems, such as ext4, JFS, ReiserFS, and XFS, but ext3 has a significant advantage in that it allows in-place upgrades from ext2 without having to backup and restore data. Benchmarks suggest that ext3 also uses less CPU power than ReiserFS and XFS.

### Main Features:
- Ext3 file system was introduced in 2001 and same was integrated in Kernel 2.4.15 with journaling feature.
- Maximun file size is **16GB - 2TB**
- Provide facility to upgrade from Ext2 to Ext3 file systems without having to back up and restore data.
# What is Ext4?
The **ext4** journaling file system also called as **fourth extended filesystem** is a journaling file system for Linux, developed as the successor to ext3. It is the default file system for most Linux distributions. 

ext4 is backward-compatible with ext3 and ext2, making it possible to mount ext3 and ext2 as ext4. This will slightly improve performance, because certain new features of the ext4 implementation can also be used with ext3 and ext2, such as the new block allocation algorithm, without affecting the on-disk format.

### Main Features:
- On October 2008, Ext4 as stable code were merged in the Kernel 2.6.28 which contains Ext4 file system.
- Maximun file size is **16GB - 16TB**
- Backward compatibility.
- Other features like Sub Directory Scalability, Multiblock Allocation, Delayed Allocation, Fast FSCK etc.

## Source:
- Wikipedia 
    - [File System](https://en.wikipedia.org/wiki/File_system)
    - [ext2](https://en.wikipedia.org/wiki/Ext2)
    - [ext3](https://en.wikipedia.org/wiki/Ext3)
    - [ext4](https://en.wikipedia.org/wiki/Ext4)
- Tecmint [Main features](https://www.tecmint.com/what-is-ext2-ext3-ext4-and-how-to-create-and-convert-linux-file-systems/)
