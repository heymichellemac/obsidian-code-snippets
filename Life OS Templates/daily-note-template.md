# <% tp.date.now("dddd Do MMM YYYY", 0, tp.file.title, "YYYY-MM-DD") %>

## 🏆 Daily Highlight
- [ ] 

## 📅 Daily Log
- 

---

## 🟠 Weekly Goals

![[W-<% tp.date.now("YYYYMM") %>-<% tp.date.now("ww") %>#✅ This Week's Goals - Mon]]

---

## 🚀 Creating
### Up Next:
```dataview
List
table category as Category
from #cc 
WHERE !contains(file.name, "Template")
AND status = "#status/upnext"
sort category asc
```

```button
name Open Todoist Writing Topics
type link
class obsidian-button
action todoist://project?id=2253952003
```

---

## 👩‍💻 Consuming

### Literature Notes

```dataview
list 
from #literature and #status/inprogress 
WHERE !contains(file.name, "Template")
sort file.name asc
Limit 10
```

```button
name Open Notion Library
type link
class obsidian-button
action https://www.notion.so/
```

---


