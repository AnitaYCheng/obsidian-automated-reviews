#journal/Monthly 
Last month：[[<%moment().subtract(1, 'M').format('YYYY-MM')%>]] || Next month：[[<%moment().add(1, 'M').format('YYYY-MM')%>]]
This quarter：[[<%moment().subtract(1,'Q').format('YYYY-[Q]Q')%>]]
Week of the month：[[<% moment().subtract(4, 'w').format('YYYY-[W]ww') %>]] || [[<% moment().subtract(3, 'w').format('YYYY-[W]ww') %>]] || [[<% moment().subtract(2, 'w').format('YYYY-[W]ww') %>]] || [[<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>]] || [[<% moment().format('YYYY-[W]ww') %>]]

## Habits
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week", 
row["Regular reviews"] as "📝",
row["Note making weekly"] as "🗒️",
FROM #journal/Weekly 
WHERE (
	file.name = "<% moment().subtract(4, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
### Habits monthly review
- Reviews monthly:: 
- Note making monthly:: 

## Mood review
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week", 
row["AM weekly mood"] as "🌅",
row["PM weekly mood"] as "🌆"
FROM #journal/Weekly 
WHERE (
	file.name = "<% moment().subtract(4, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
**Mood monthly review**::<br>-


## Identities review
What work did you do to your identities this month?
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week",
row["IDExample days"] as "IDExample",
row["IDExample2 days"] as "IDExample2"
from #journal/Weekly
WHERE (
	file.name = "<% moment().subtract(4, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().format('YYYY-[W]ww') %>"
)
SORT file.name asc
```



## Weekly reviews

### Task achievement review

#### Weekly Big 3 
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week", 
row["Tactics-achievement-score"] as "Tactic achievement score"
WHERE (
	file.name = "<% moment().subtract(4, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
**Weekly Big 3 review**::<br>- 

### Memorable
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week", 
row["Memorable"] as "Memorable"
WHERE (
	file.name = "<% moment().subtract(4, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
**Memorable monthly review**::<br>-

### Takeaways
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week", 
row["Takeaways"] as "Takeaways"
WHERE (
	file.name = "<% moment().subtract(4, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
**Takeaways monthly review**::<br>-

### Start, continue, or stop
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week", 
row["Start"] as "Start",
row["Continue"] as "Continue",
row["Stop"] as "Stop"
WHERE (
	file.name = "<% moment().subtract(4, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
**Start/continue/stop monthly review**::<br>-

## Thoughts on this month

^thoughtsOnThisMonth

## Planning

![[<% moment().subtract(1, 'years').format('YYYY') %>#Priorities for <% moment().format('YYYY') %>]]

![[<% moment().subtract(1, 'years').format('YYYY') %>#Goals for <% moment().format('YYYY') %>]]

![[<% moment().subtract(1, 'Q').format('YYYY-[Q]Q') %>#Priorities for <% moment().format('YYYY-[Q]Q') %>]]

![[<% moment().subtract(1,'months').format('YYYY-MM') %>#Priorities for <% moment().format('YYYY-MM') %>]]

### Priorities for <%moment().add(1, 'M').format('YYYY-MM')%>
1. 