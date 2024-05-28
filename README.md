# dummy
Some dummy repo for testing.

To download and install:
```
git clone https://github.com/sitemapxml/dummy.git /usr/local/test
cd /usr/local/test
rm -rf .git/ LICENSE README.md
```

There should be 9 files in total:
```
find -type f | wc -l
9
```

This should be the full list:
```
ls -A1lh
total 36K
-rw-r--r-- 1 root root  1 May 23 18:14 9-files-in-total
-rw-r--r-- 1 root root  1 May 23 18:14 double.extension.empty
-rw-r--r-- 1 root root 52 May 23 18:14 double.extension.not_empty
-rw-r--r-- 1 root root  1 May 23 18:14 .empty_dotfile
-rw-r--r-- 1 root root  1 May 23 18:14 empty_file_no_extension
-rw-r--r-- 1 root root  1 May 23 18:14 empty-file.txt
-rw-r--r-- 1 root root 34 May 23 18:14 .not_empty_dotfile
-rw-r--r-- 1 root root 48 May 23 18:14 not_empty_no_extension
-rw-r--r-- 1 root root 31 May 23 18:14 test-file-not-empty.txt
```

This should be the list of empty files:
```
find -type f -size 0
./empty-file.txt
./double.extension.empty
./9-files-in-total
./.empty_dotfile
./empty_file_no_extension
```

And this should be the list of not empty files:
```
find -type f -size +0
./double.extension.not_empty
./test-file-not-empty.txt
./.not_empty_dotfile
./not_empty_no_extension
```
