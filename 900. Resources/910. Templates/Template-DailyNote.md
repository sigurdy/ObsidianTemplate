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
> TABLE file.name AS Name, file.ctime AS Created, file.mtime AS Modified
> FROM ""
> WHERE file.cday = date(today) OR file.mday = date(today)
> SORT file.mtime DESC
> ```

# 📆 Meetings

> [!WARNING] Coming Meeting
> ```dataview
> TABLE meetingDate AS MeetingDate, file.cday AS DateCreated
> FROM "" AND !"900. Resources"
> WHERE meetingDate AND meetingDate >= date(today)
> SORT meetingDate DESC
> LIMIT 5
> ```


> [!WARNING] Last Meetings
> ```dataview
> TABLE meetingDate AS MeetingDate, file.cday AS DateCreated
> FROM "" AND !"900. Resources"
> WHERE meetingDate AND meetingDate <= date(today)
> SORT meetingDate DESC
> LIMIT 5
> ```

# 🎯 Actions



# 📝 Notes





