# centos_find_and_replace

```
find /path/to/folder/ -type f -name "*.php" -exec sed -i 's/10.15.20.15/10.15.20.5/g' {} +
```

In there:

find /path/to/folder/ will search all files in /path/to/folder/ directory and subdirectories.
-type f specifies that to search only real files (not directories).
-name "*.php" specifies that only files with the .php extension should be searched.
-exec sed -i 's/10.15.20.15/10.15.20.5/g' {} + will replace the string “10.15.20.15” with the string “10.15.20.5” in all files search.
