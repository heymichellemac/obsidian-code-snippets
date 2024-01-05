# W-{{DATE:YYYYMM}}-{{DATE:ww}} 
Year:: [[Y-{{DATE:YYYY}}]]
Quarter:: [[Q-{{DATE:YYYY-Q}}]]
Category:: #weekly

## ⏰ Weekly review prep
### Prep Tasks
- [ ] Clear desk
- [ ] Clear downloads
- [ ] Check for updates
- [ ] Email
- [ ] Calendar
- [ ] Consolidate daily notes from the last week

### 🔃 Last Week
![[W-<% tp.date.now("YYYYMM") %>-<% tp.date.now("ww"), -1 %>#💬 Reflections]]

---

## 💬 Reflections 

### 🌹 What Went Well This Week?

### 🌵 What Should I Stop Doing?

### 🌱 What Could Be Improved?

---
## 🟠 Planning the week ahead
### Current goals

```dataview
	LIST
	FROM #goal
	WHERE contains(Quarter, [[Q-{{DATE:YYYY}}-{{DATE:Q}}]])
	SORT file.name DESC
```

### Current projects
```dataview
	LIST
	FROM #project
	WHERE contains(Quarter, [[Q-{{DATE:YYYY}}-{{DATE:Q}}]])
	AND !contains(Status, "#status/done")
	SORT file.name DESC
```

### This week

> [!question]- 3 goals to accomplish this week
> List 3 goals to accomplish this week (look at making progress towards goals as a priority)

- [ ] 
- [ ] 
- [ ] 

