# dummy
Some dummy repo for testing.

```
cd /usr/local
git clone https://github.com/sitemapxml/dummy.git ./test
cd test
rm -rf .git/ LICENSE README.md
```

```
ls -A1lh
total 36K
-rw-r--r-- 1 root root  1 May 23 18:14 9-files-in-total
-rw-r--r-- 1 root root  1 May 23 18:14 double.extension.empty
-rw-r--r-- 1 root root  1 May 23 18:14 double.extension.not_empty
-rw-r--r-- 1 root root  1 May 23 18:14 .empty_dotfile
-rw-r--r-- 1 root root  1 May 23 18:14 empty_file_no_extension
-rw-r--r-- 1 root root  1 May 23 18:14 empty-file.txt
-rw-r--r-- 1 root root 34 May 23 18:14 .not_empty_dotfile
-rw-r--r-- 1 root root 48 May 23 18:14 not_empty_no_extension
-rw-r--r-- 1 root root 31 May 23 18:14 test-file-not-empty.txt
```

```
find -type f -size 0
./empty-file.txt
./double.extension.empty
./9-files-in-total
./.empty_dotfile
./empty_file_no_extension

find -type f -size +0
./double.extension.not_empty
./test-file-not-empty.txt
./.not_empty_dotfile
./not_empty_no_extension
```
