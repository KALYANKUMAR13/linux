<img width="599" alt="image" src="https://github.com/user-attachments/assets/c7413d94-a0c0-40ad-9c5f-2d87782e58a9" />

Each pic or file gets inode (group of inodes) and it is scattered across the disk in storage. So innode helps to associate it to the particular file.
It also keeps the metadata, like last modified, permissions and last accessed.  We can remember the inodes. When we create a file, it creates a link. that link associates the file path and actucal file in storeage(INODE) .This is hard link.


If a file is in /home/kalyan/picture/1.png directory,

If some other user /home/mano/picture/1.png want the same file, Insead of copying, create a hard link referencing to that pic 
```
ln /home/kalyan/picture  /home/mano/picture/1.png
```

It will not create a new file with copied contents, but rather link the two paths to the same underlying inode (file data).

Both paths will behave like the same file: modifying one will affect the other.

If you delete one of them, the data is still safe as long as at least one hard link remains.

Requirements:
Hard links must be on the same filesystem. If /home/kalyan and /home/mano are on different partitions, the command will fail.


If either of one deletes the file, tha another can still can view the file, (the file will reduce teh hard link to 1, instead to 2). If both deletes, then we can't get hte data.


LIMITATIONS:

we can only hardlinks the files not the directories.

Can be done on same filesystem , not on different file system  (/home/aaraon/file -- /mnt/file/backup)
