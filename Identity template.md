## My why

## Origins

## Current progress
```dataview

TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Year",
row["Mentor annual review"] as "Review"

FROM #journal/Yearly and "Personal reviews" and -#M/About

sort file.cday descending

limit 1

```
```dataview

TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Quarter",
row["Mentor quarterly review"] as "Review"

FROM #journal/Quarterly and "Personal reviews" and -#M/About

SORT file.name desc

limit 4
```