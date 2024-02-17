---
date: {{date}} {{time}}
aliases: 
tags:
- IsProject
up: "[[_Dashboard.canvas|_Dashboard]]"
---


# 📃 Documentation


# 🏗️ Infrastructure
| Server Name | Type | Environment |
| ---- | ---- | ---- |
|  |  |  |

# 🔗 Related Notes


> [!ERROR] Update Filter for the below Query
> The query below query all files in the vault This need to be updated on the spesifics from this project, e.g., `FROM #project/projectName AND !"900. Resources"`.


> [!tldr]- Related Notes
> ```dataview
> TABLE file.mtime AS Modified, file.cday AS DateCreated, aliases AS Alias
> FROM ""  AND !"900. Resources"
> WHERE file.name != this.file.name 
> SORT file.mtime DESC
> LIMIT 10
> ```