# To unzip a zip file in unix


```c
unzip archive.zip

```
## You can also extract it to a specific directory

you will use `-d` to specifiy the path

```c
unzip archive.zip -d ~/new/folder/one/

```
you can also uzip only a specific file from a zip
```c
unzip archive.zip file.txt -d destination_folder

```
only the `file.txt` will be extracted from the folder

#To make zip for a file or folder
first move all your files and folders into one folder

```c
zip -r archive.zip folder

```

for tar,gzip,rar etc

```c
tar -zcvf archive_name.tar.gz folder_to_compress

```

This will create a compressed archive with .tar.gz extension and it is also possible to compress using .tar.bz2 or .tar.xz

```c
tar -jcvf archive_name.tar.bz2 folder_to_compress

```
```c
tar -Jcvf archive_name.tar.xz folder_to_compress

```


## How to view the content of a zip without extracting the zip file

You can view the contents of a zip file without extracting it using the command line tool "unzip" with the option "-l" (for "list"). The basic syntax for listing the contents of a zip file is:

```c
unzip -l archive.zip

```

Another way is to use the command line tool "zipinfo". The basic syntax for listing the contents of a zip file is:


```c
zipinfo archive.zip

```
And also you can use the command line tool "less" to display the contents of a zip file, this is useful when the zip file is very large and you want to navigate through it page by page.


```c
less archive

```
then type


```c
y
```
it will display it as binary.


## How to unzip password protected zip file using unix

```c
unzip -P enter_password archive.zip

```
## How to create  your zip file with password

```c
zip -e archive.zip file_or_folder

```

# Note
if you want to add multiple files_folders you can use `r` to add recursively

```c
zip -r archive.zip file1, folder1, file2, folder2

```

## you can also add a file_folder to an already existing folder using `-u`

```c
zip -u archive.zip file_folder

```
 
you can also add multiple files using recursively `-ur`

```c
zip -ur archive.zip file1, folder1, file2, folder2

```






