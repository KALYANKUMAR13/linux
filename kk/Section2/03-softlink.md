IN windows, when we install a software , we gets a shortcut to desktop ,and when we click it , it opens a software,

But actually, it goes to the exe file the software in  C:/Program File/vscode/terminal/code.exe

Softlinks are similar to this.

Hardlink points to INODE, where softlink points to filepath insttead of inode. SoftLink is also know as symolic link

ln -s /target /neededfile
ln -s /target(existingfile) /neededfile(created)


In softlink, the permission dosen't matter, so the soft link gets 777.


When the target file gets changed its file path, softlink will break,it can't access it.

We can do softlinks to directories.
