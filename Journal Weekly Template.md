For week ending [[<% moment().endOf('week').format('YYYY-MM-DD') %>]]

#journal/Weekly 
Last week：[[<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>]] || Next week：[[<% moment().add(1, 'w').format('YYYY-[W]ww') %>]]
Last month: [[<% moment().subtract(1, 'M').format('YYYY-MM') %>]] || This month：[[<% moment().format("YYYY-MM") %>]]

## Weekly review

### Habits
```dataview
table 
row["Review"] as "✅",
row["Note making"] as "🗒️",
FROM #journal/Daily 
WHERE (
file.name = "<% tp.date.weekday("YYYY-MM-DD", 0) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 1) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 2) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 3) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 4) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 5) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 6) %>"
)
SORT file.name asc
```

#### Habits weekly review
- Regular reviews:: 
- Note making weekly:: 

---


#### Last weekly big 3
| How far did you go? | Percent completed |
|-----|------|
| `= [[<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>]].Big3-1` | Percent |
| `= [[<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>]].Big3-2` | Percent |
| `= [[<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>]].Big3-3` | Percent | 

**Tactics-achievement-score**::
**Last week's tactics achievement score:** `= [[<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>]].Tactics-achievement-score`


### Summaries
![[<% tp.date.weekday("YYYY-MM-DD", 0) %>#^quickSummary]] 
![[<% tp.date.weekday("YYYY-MM-DD", 1) %>#^quickSummary]] 
![[<% tp.date.weekday("YYYY-MM-DD", 2) %>#^quickSummary]] 
![[<% tp.date.weekday("YYYY-MM-DD", 3) %>#^quickSummary]] 
![[<% tp.date.weekday("YYYY-MM-DD", 4) %>#^quickSummary]] 
![[<% tp.date.weekday("YYYY-MM-DD", 5) %>#^quickSummary]] 
![[<% tp.date.weekday("YYYY-MM-DD", 6) %>#^quickSummary]]

**Memorable**::<br>- 

---

## Mood
```dataview
table 
row["AM Mood"] as "🌅",
row["PM Mood"] as "🌆"
FROM #journal/Daily 
WHERE (
file.name = "<% tp.date.weekday("YYYY-MM-DD", 0) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 1) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 2) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 3) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 4) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 5) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 6) %>"
)
SORT file.name asc
```

### Mood and health weekly review
- AM weekly mood::
- PM weekly mood::


## Five Minute Journal
```dataview
table 
row["I am grateful for"] as Gratitude, 
row["What went well"] as "Good", 
row["What could have gone better"] as "Could improve", 
row["Things I learned"] as "TIL"
FROM #journal/Daily 
WHERE (
file.name = "<% tp.date.weekday("YYYY-MM-DD", 0) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 1) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 2) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 3) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 4) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 5) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 6) %>"
)
SORT file.name asc
```
---

## Weekly takeaways

### What worked? What didn't? What affected your performance?
🤩  Great!
- 

😰  Didn't work so well
- 

🤔  Thinking about what happened
- 

**Start**::<br>- 
**Continue**::<br>- 
**Stop**::<br>- 
**Takeaways**:: <br>- 

---

### Identities Review
*What work did you do on your identities this week?*

#### [[IDExample]]
**IDExample days**:: /7
**IDExample review**::<br>- 


#### [[IDExample2]]
**IDExample2 days**:: /7
**IDExample2 review**::<br>- 


---

## Weekly planning

### Major things ahead
Refer to your calendar and goals. What will (or should) happen this coming week?
- 


### Intention setting
**Priorities**::<br>- 
**Possible obstacles**::<br>- 
**Events**::<br>- 

![[<% moment().subtract(1, 'years').format('YYYY') %>#Goals for <% moment().format('YYYY') %>]]

![[<% moment().subtract(1, 'Q').format('YYYY-[Q]Q') %>#Priorities for <% moment().format('YYYY-[Q]Q') %>]]

![[<% moment().subtract(1,'months').format('YYYY-MM') %>#Priorities for <% moment().format('YYYY-MM') %>]]


### Weekly Big 3
List 3 items you must accomplish this week to advance your goals or projects
1. **Big3-1**::
2. **Big3-2**::
3. **Big3-3**::
