# A collection of grep command

> Find a literal expression recursively in the current directory by a single file extension type, then print the results lines and the files name:

```bash
$ grep -Hrn "search term" --include '*.ext*' ./
```
- `-H`                       causes the filename to be printed
- `-r`                       does a recursive search
- `-n`                       causes line number to be printed
- `-- include '*.ext*'`      only consider a single given file extension 
- `--include=*.{js,scss}`    can be multiple extensions
- `.` or `./`                current directory path
- `path/to/files `           can be a specific path

Further options:

- `-i`                        do a case-insensitive search
- `--exclude-dir=dir`         useful for excluding directories like .svn and .git