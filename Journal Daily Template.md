#journal/Daily 
Yesterday：[[<% moment().subtract(1, 'd').format('YYYY-MM-DD') %>]] || Tomorrow：[[<% moment().add(1, 'd').format('YYYY-MM-DD') %>]]
This week：[[<% moment().format('YYYY-[W]ww') %>]] 
Past year: [[<% moment().subtract(1, 'years').format('YYYY') %>]]

## Weekly intentions

![[<% moment().subtract(1,'w').format('YYYY-[W]ww') %>#Weekly Big 3]]

```dataview
table without id

row["Priorities"] as "Priorities",
row["Possible obstacles"] as "Obstacles",
row["Events"] as "Events"

WHERE (
file.name = "<% moment().subtract(1,'w').format('YYYY-[W]ww') %>"
)
```

## Remember from last week
```dataview
table without id

row["Start"] as "Start",
row["Continue"] as "Continue",
row["Stop"] as "Stop"

WHERE (
file.name = "<% moment().subtract(1,'w').format('YYYY-[W]ww') %>")
```

```dataview
table without id

row["Takeaways"] as "Takeaways"

WHERE (
file.name = "<% moment().subtract(1,'w').format('YYYY-[W]ww') %>")
```

---

## Today

**Daily Big 3**::<br>1. <br>2. <br>3. 


### Habits
- AM Mood:: 
- PM Mood:: 
- Review:: 
- Note making:: 

---
## Daily Review
### 5MJ
- I am grateful for::<br>1. <br>2. <br>3. 

- What went well::<br>1. <br>2. <br>3. 

- What could have gone better::<br>1. <br>2. <br>3. 

- Things I learned:: <br>1. <br>2. 

---
### Created today
```dataview
TABLE file.folder AS "Folder"
WHERE file.cday = date(<% moment().format('YYYY-MM-DD') %>)
SORT file.folder desc
```




