# {{title}}
Theme: 

Quarters:
```dataview
list
from "01-life-os/02-quarters"
where contains(file.name, "{{date:YYYY}}")
sort file.name asc
```

Goals:
```dataview
list
from "01-life-os/03-goals"
where theYear = "{{date:YYYY}}"
sort file.name asc
```

Projects:
```dataview
list
from "01-life-os/04-projects"
where theYear = "{{date:YYYY}}"
sort file.name asc
```

---

## Year End Review
### Review Of The Past Year
-   How did my yearly theme help me this year?
-   What went really well this year?
-   What surprised me?
-   What am I most proud of accomplishing?
-   What challenged me?
-   What am I most grateful for?
-   What have I learned this year?
-   My top 5 favorite things from this year
-   Describe this year in 3 words

### Looking Ahead To Next Year
-   What is my yearly theme and why?
-   What am I most looking forward to next year?
-   What am I feeling apprehensive about?
-   What do I want to do differently?
-   What area of y life to I most want to develop?
-   What do I want to accomplish next year?
-   What challenges am I likely to face?

### Taking Action
-   I will make more time for:
-   I will learn about:
-   I will say NO to:
-   I will say YES to: