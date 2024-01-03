#journal/Yearly
Past year：[[<% moment().subtract(1, 'years').format('YYYY') %>]] || Next year：[[<% moment().add(1, 'years').format('YYYY') %>]]
3-year vision: [[2024 vision work]]
Quarters of this year：[[<%moment().subtract(3,'Q').format('YYYY-[Q]Q')%>]] || [[<%moment().subtract(2,'Q').format('YYYY-[Q]Q')%>]] || [[<%moment().subtract(1, 'Q').format('YYYY-[Q]Q')%>]] || [[<%moment().format('YYYY-[Q]Q')%>]] 


## Reviews
### Habits by quarter
```dataview
table 
row["Habits quarterly review"] as "Habits"
WHERE (
file.name = "<% moment().subtract(3, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().subtract(2, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().subtract(1, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().format('YYYY-[Q]Q') %>"
)
SORT file.name asc
```
**Habits annual review::**<br>- 


### Identity goals by quarter
#### [[IDExample]]
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Quarter",
row["IDExample quarterly review"] as "Review"
WHERE (
file.name = "<% moment().subtract(3, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().subtract(2, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().subtract(1, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().format('YYYY-[Q]Q') %>"
)
SORT file.name asc
```
**IDExample annual review**:: <br>- 

#### [[IDExample2]]
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Quarter",
row["IDExample2 quarterly review"] as "Review"
WHERE (
file.name = "<% moment().subtract(3, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().subtract(2, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().subtract(1, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().format('YYYY-[Q]Q') %>"
)
SORT file.name asc
```
**IDExample2 annual review**:: <br>- 



### Memorable things by quarter
```dataview
table 
row["Memorable quarterly review"] as "Memorable"
WHERE (
file.name = "<% moment().subtract(3, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().subtract(2, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().subtract(1, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().format('YYYY-[Q]Q') %>"
)
SORT file.name asc
```

### Takeaways by quarter
```dataview
table 
row["Start/continue/stop quarterly review"] as "Start/Stop/Continue",
row["Takeaway quarterly review"] as "Takeaways"
WHERE (
file.name = "<% moment().subtract(3, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().subtract(2, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().subtract(1, 'Q').format('YYYY-[Q]Q') %>" or
file.name = "<% moment().format('YYYY-[Q]Q') %>"
)
SORT file.name asc
```




---

### Domain review
#### 💰 Finances
- **What big financial milestone came through?**

- **How has my relationship with money improved?**

- **Did certain purchases and experiences make me smile?**

- **What financial milestone do I hope for next year?**

- **How do I hope my relationship with money will improve this year?**


#### 👼🏻 Child
- **How did I enable my child to thrive?**

- **What do I hope for my child next year?**


#### 🧳 Colleagues
- **How did I enable colleagues to thrive?**

- **How can I enable my colleagues to thrive this coming year?**


#### 🧠 Learning and skills
- **What big breakthroughs did I learn? Where did I learn them?**

- **What do I hope to learn this year?**


#### 👩🏻‍⚕️ Health
- **How has my health been?**

- **What habits helped support that?**

- **How do I hope my health will improve this year?**

- **Which habits can I nurture to support that?**


#### ❤️ Spouse
- **How did I enable my partner to thrive?**

- **How can I help support partner this year?**

- **What do I want out of the marriage this coming year?**


#### 🧘🏻‍♀️ Emotional well-being
- **What did I confront that I'd been avoiding?**

- **What problems do I still have yet to confront?**


---

## 🎯 Priorities and goals for the next year

>[! Question]
>Who do I want to become?

>[! Tip]
>Go for "MT" goals as proxies for outcomes - measurable and time-based. Focus on targets. Don't be afraid to "eliminate."

### Review of past vision goals
![[2024 vision work]]

### Priorities for <% moment().add(1, 'years').format('YYYY') %>

1. 


### Goals for <% moment().add(1, 'years').format('YYYY') %>
Max 8 goals, assign max 3 to work on per quarter

1. 
