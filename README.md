# essential-admin-task-snippets
Some tasks are optional but this are essential


## Find the biggest node_modules folder
``` 
find ~/  -type d -not -path "*/node_modules/*" -iname "node_modules" > folder_scan.txt && cat folder_scan.txt | xargs du -sh | sort -h
```

## Find files without errors that are bigger then 1GB
```
find . -type f -size +1G -exec du -h {} \; 2>&1 | grep -v "’: "
``` 
