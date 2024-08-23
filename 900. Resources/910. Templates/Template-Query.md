> [!ERROR]
> Add `dataview` at the top of the code below in order for it to compile. Also change `FROM #yourtag AND !"900. Resources"` to use the tags you want to query.

```
TABLE file.mtime AS Modified, file.cday AS DateCreated, aliases AS Alias
FROM #yourTag AND !"900. Resources"
WHERE file.name != this.file.name 
SORT file.mtime DESC
LIMIT 10
```