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
### Article Ideas:
```dataview
List
from "05-content-creation/03-articles" 
where Status = "#status/backlog" 
or Status = "#status/inprogress"
sort file.name asc
Limit 10
```
```button
name Open Todoist Writing Topics
type link
class obsidian-button
action todoist://project?id=2253952003
```

### Upcoming Newsletter Editions:
```dataview
list
from "05-content-creation/09-design-insight-newsletter" and #status/inprogress  
sort file.name asc
Limit 5
```

### Twitter Thread Ideas:
```dataview
List
from "05-content-creation/02-threads/thread-ideas" 
where Status = "#status/backlog" 
or Status = "#status/inprogress"  
sort file.name asc
Limit 10
```
```button
name Open Tweet HUD
type link
class obsidian-button
action https://www.notion.so/Tweet-HUD-6c5cfb6086db4721a1798cb71121ce3f
```
---

## 👩‍💻 Consuming
```button
name Process Notion Inbox
type link
class obsidian-button
action https://www.notion.so/Inbox-b6d197922a83427591321ae667c04fb3
```
```button
name Open Notion Library
type link
class obsidian-button
action https://www.notion.so/98ab63eeef8946c9931362aa8d429e2e?v=555da457e8714c888b76cf7b37397201
```

---

## 💬 Thoughts + Ideas
### Process Literature Notes:
```dataview
list 
from "02-literature" and #status/inprogress  
sort file.name asc
Limit 3
```
### Review Evergreen Notes:

<% tp.file.include("[[📄 Random Evergreen Note Template]]") %>

---
