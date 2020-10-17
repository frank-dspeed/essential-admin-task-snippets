# essential-admin-task-snippets
Some tasks are optional but this are essential


## Find the biggest node_modules folder
``` 
find ~/  -type d -not -path "*/node_modules/*" -iname "node_modules" > folder_scan.txt && cat folder_scan.txt | xargs du -sh | sort -h
```
