---
type: template
subject: <% tp.file.title %>
status: 🏗️ In Progress
---
# 🗺️ <% tp.file.title %> Map of Content

> [!info] **Learning Goal**
> *Master the syntax and core libraries of <% tp.file.title.replace(" MOC", "") %>.*

---

## 📑 Automated Note Index
*The table below updates automatically using the Dataview plugin.*

```dataview
TABLE date as "Date", status as "Progress"
FROM "<% tp.file.folder() %>"
WHERE type = "study-note"
SORT date DESC
```
[[Master Index]]