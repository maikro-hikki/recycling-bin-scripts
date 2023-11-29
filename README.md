# Recycling Scripts in UNIX
- Two scripts, `recycle` and `restore`, that can replace the remove (`rm`) command to reduce risk of information loss
---
## Recycle Script
- The recycle script accepts the name of a file as a command line argument as the `rm` command does in UNIX, but instead of deleting the file, the script moves it to a recycle bin directory called recyclebin in the home directory
- The script can also recycle multiple files, ex. `bash recycle file1 file2 file3`
### Just like the `rm` command, the recycle script can use the `–i`, `–v`, and `–r` options,
- `–i` for interactive mode
- `–v` option for verbose mode
- `–r` option to recycle directories and their contents
- All options can be used at the same time where applicable
---
## Restore Script
- The restore script restores recycled files back to their original location
- For the file to be restored, use the file name with their inode number in order to restore the file, ex. `bash restore f1_1234`
