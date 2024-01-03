#journal/Quarterly 
Last quarter：[[<%moment().subtract(1, 'Q').format('YYYY-[Q]Q')%>]] || Next quarter：[[<%moment().add(1,'Q').format('YYYY-[Q]Q')%>]]
Month of the quarter：[[<% moment().subtract(2, 'M').format('YYYY-MM') %>]] || [[<% moment().subtract(1, 'M').format('YYYY-MM') %>]] || [[<% moment().format('YYYY-MM') %>]]
Past year：[[<% moment().subtract(1, 'years').format('YYYY') %>]]

## Projects done this quarter
```dataview
LIST 
FROM "Efforts" AND #S/Complete 
WHERE Due < date(<% moment().format('YYYY-MM-DD') %>) AND Due > date(<% moment().subtract(2, 'M').format('YYYY-MM-DD') %>)
SORT Due desc
```

## Habits review
```dataview
table 
row["Reviews monthly"] as "✅",
row["Note making monthly"] as "🗒️"
FROM #journal/Monthly 
WHERE (
	file.name = "<% moment().subtract(2, 'M').format('YYYY-MM') %>" or
	file.name = "<% moment().subtract(1, 'M').format('YYYY-MM') %>" or
	file.name = "<% moment().format('YYYY-MM') %>"
)
SORT file.name asc
```
**Habits quarterly review**:: <br>-


## Identity goals this quarter
### [[IDExample]]
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Month",
row["IDExample monthly review"] as "Review"
WHERE (
	file.name = "<% moment().subtract(2, 'M').format('YYYY-MM') %>" or
	file.name = "<% moment().subtract(1, 'M').format('YYYY-MM') %>" or
	file.name = "<% moment().format('YYYY-MM') %>"
)
SORT file.name asc
```
**IDExample quarterly review**:: <br>- 

### [[IDExample2]]
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Month",
row["IDExample2 monthly review"] as "Review"
WHERE (
	file.name = "<% moment().subtract(2, 'M').format('YYYY-MM') %>" or
	file.name = "<% moment().subtract(1, 'M').format('YYYY-MM') %>" or
	file.name = "<% moment().format('YYYY-MM') %>"
)
SORT file.name asc
```
**IDExample2 quarterly review**:: <br>- 



## Monthly reviews

### Thoughts on the month

![[<%moment().subtract(2, 'M').format('YYYY-MM')%>#^thoughtsOnThisMonth]] 

![[<%moment().subtract(1, 'M').format('YYYY-MM')%>#^thoughtsOnThisMonth]] 

![[<%moment().format('YYYY-MM')%>#^thoughtsOnThisMonth]] 


### Memorable
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Month",
row["Memorable monthly review"] as "Memorable"
WHERE (
	file.name = "<% moment().subtract(2, 'M').format('YYYY-MM') %>" or
	file.name = "<% moment().subtract(1, 'M').format('YYYY-MM') %>" or
	file.name = "<% moment().format('YYYY-MM') %>"
)
SORT file.name asc
```
**Memorable quarterly review**::<br>-

### Takeaways
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Month",
row["Takeaways monthly review"] as "Takeaways"
WHERE (
	file.name = "<% moment().subtract(2, 'M').format('YYYY-MM') %>" or
	file.name = "<% moment().subtract(1, 'M').format('YYYY-MM') %>" or
	file.name = "<% moment().format('YYYY-MM') %>"
)
SORT file.name asc
```
**Takeaway quarterly review**::<br>-


## Start/Stop/Continue

```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Month",  
row["Start/continue/stop monthly review"] as "Review"
WHERE (
	file.name = "<% moment().subtract(2, 'M').format('YYYY-MM') %>" or
	file.name = "<% moment().subtract(1, 'M').format('YYYY-MM') %>" or
	file.name = "<% moment().format('YYYY-MM') %>"
)
SORT file.name asc
```
**Start/continue/stop quarterly review**::<br>- 


## Planning
![[<% moment().subtract(1, 'years').format('YYYY') %>#Priorities for <% moment().format('YYYY') %>]]

![[<% moment().subtract(1, 'years').format('YYYY') %>#Goals for <% moment().format('YYYY') %>]]

![[<%moment().subtract(1, 'Q').format('YYYY-[Q]Q') %>#Priorities for <%moment().format('YYYY-[Q]Q')%>]]

### Priorities for <%moment().add(1,'Q').format('YYYY-[Q]Q')%>
1. 

