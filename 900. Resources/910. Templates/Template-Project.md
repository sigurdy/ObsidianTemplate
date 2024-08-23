---
date: {{date}} {{time}}
aliases: 
tags: 
up: "[[_Dashboard.canvas|_Dashboard]]"
---

> [!ERROR] ## Fix the following:
> The query below query all files in the vault.
>  - Update the tag of this file to be e.g., `#project/<myproject>`
> - In the query below in "Related Notes". Edit the filter to specify `FROM #project/<myproject> AND !"900. Resources"`

# 📃 Documentation


# 🔗 Related Notes


> [!tldr]- Related Notes
> ```dataview
> TABLE file.mtime AS Modified, file.cday AS DateCreated, aliases AS Alias
> FROM #project  AND !"900. Resources"
> WHERE file.name != this.file.name 
> SORT file.mtime DESC
> LIMIT 10
> ```