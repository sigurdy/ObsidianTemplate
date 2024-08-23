---
date: {{date}} {{time}}
aliases: 
tags:
  - DailyNote
up: "[[_Dashboard.canvas|_Dashboard]]"
---

# ✅ Tasks

> [!warning] Task Not Done
> ```dataview
> TASK 
> FROM ""
> WHERE !completed
> GROUP BY file.link
> ```
# 🗒️ Notes Created or Modified This Day
> [!NOTE]
> ```dataview
> TABLE file.name AS Name, file.cday AS DateCreated, file.mday AS DateModified
> FROM ""
> WHERE file.cday = date(today) OR file.mday = date(today)
> ```

# 🎯 Actions



# 📝 Notes





