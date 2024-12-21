---
date: {{date}} {{time}}
aliases: 
tags:
  - DailyNote
up: "[[_Dashboard.canvas|_Dashboard]]"
---

# 📝 Notes



# 📆 Meetings

> [!WARNING] Coming Meetings
> ```dataview
> TABLE meetingDate AS MeetingDate, file.cday AS DateCreated
> FROM "" AND !"900. Resources"
> WHERE meetingDate AND meetingDate >= date(today)
> SORT meetingDate DESC
> LIMIT 10
> ```


> [!WARNING] Previous Meetings
> ```dataview
> TABLE meetingDate AS MeetingDate, file.cday AS DateCreated
> FROM "" AND !"900. Resources"
> WHERE meetingDate AND meetingDate < date(today)
> SORT meetingDate DESC
> LIMIT 10
> ```

# 🗒️ Notes Created or Modified This Day
> [!NOTE]
> ```dataview
> TABLE file.name AS Name, file.ctime AS Created, file.mtime AS Modified
> FROM ""
> WHERE file.cday = date(today) OR file.mday = date(today)
> SORT file.mtime DESC
> ```

# ✅ Tasks

> [!warning] Task Not Done
> ```dataview
> TASK 
> FROM ""
> WHERE !completed
> GROUP BY file.link
> ```





