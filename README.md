# My automated review system

This system is what I use every day to track if things I'm trying are working  over time, especially with my ADHD tendencies.

At this point in my life, it's less about productivity and achievement. For me, it's more about acting with intention. while accepting the way my brain works. And I figure, you can't act with intention unless you can properly see what you've done in the past.

This system allows me to see what I've learned, what worked well, and what could have worked better at a glance even from the beginning of the year.

## Inspiration
Inspired by [Mason Royal's presentation at Linking Your Thinking](https://youtu.be/LowOdmZLF1E?si=5Qa4uwrlN533ap_p&t=929), I modified his [Automated Review Roll ups](https://github.com/masonroyal/obsidian-reviews) to better align with my goal of intention.

I also added elements from the [Full Focus planner system](https://fullfocus.co/) and [12 Week Year](https://12weekyear.com/) for my daily and weekly reviews, as well as goal setting. I was also inspired by [RadReads](https://radreads.co/productivity/) for some content in the yearly reviews.

## Requirements
The "journal" templates that make up the review system. The vision, goals, and habits templates helps support your intention work. Place all of these into your templates folder in your Obsidian setup.

You will need to have [Obsidian](https://obsidian.md/) and the plugins [Dataview](https://github.com/blacksmithgu/obsidian-dataview) and [Templater](https://github.com/SilentVoid13/Templater) installed.

### The question of tasks
Mason's templates (and my own personal working system) also include [Tasks](https://github.com/obsidian-tasks-group/obsidian-tasks) and task reviews, but I have removed the task system from these templates to simplify things. I may develop a separate post about task management later.

## How the automated system works
**Daily** reviews roll up to **weekly** reviews, which roll up to **monthly** reviews, which roll up to **quarterly** reviews, which roll up to **yearly** reviews. I use each review as an opportunity to summarize my logs from the previous period. This is how I'm able to see what I was thinking about months ago.

Here is an example of how I log habits in a daily review file:

<img width="653" alt="A bulleted list of habit labels like AM Mood, PM Mood, Review, Note making, Music, Read, with all labels followed by a double colon. There is an emoji attached to some of the items." src="https://github.com/AnitaYCheng/obsidian-automated-reviews/assets/6760632/e07912cd-9ba0-49a1-8b75-ce84dc7ad680">

Here's how my daily habits are visible in the weekly review, and how I can use it to summarize how I did on my habits every day:

<img width="646" alt="A table where the rows are daily file titles like 2023-06-11 and the columns are emojis assigned to certain habits. Each cell either shows the emoji assigned to that day's habit, or a dash if it was empty a.k.a. not done. Underneath is a new bulleted list with the habit labels denoting it as a weekly summary." src="https://github.com/AnitaYCheng/obsidian-automated-reviews/assets/6760632/7bd96733-a28b-462d-bdfa-2572a7eb442d">

### Populating the templates
I've left these templates with placeholder habits and identities, so you can track where in the templates to modify them. You'll also likely need to learn a bit of how [Dataview works](https://blacksmithgu.github.io/obsidian-dataview/queries/data-commands/) so you can modify any queries to your liking.

### Scheduling the reviews
Using Moment.js syntax with the Templater plugin means you don't have to calculate any dates when you create a new file. Just click through to a new date, fire up Templater, select the template you want, and it'll do the job!

But this also means that you need to schedule the reviews on time. Otherwise you'll need to edit some of the calculated dates. Not a dealbreaker, but definitely annoying.

You should create each review file from its corresponding template before midnight on the last day before the stated period is over. For example:
- Daily reviews before the referenced day is over (meaning, 11:59 pm local time)
- Weekly reviews before Saturday is over in the referenced week
- Monthly reviews before the last day is over in the referenced month
- Quarterly reviews on the last day of the referenced quarter
- Yearly reviews before January 1

You can create the files beforehand for weekly or monthly reviews as long as you're in the referenced time period, but they won't populate with your content until there's something to roll up.

## Supporting templates
I've included templates for goal-setting, habit setting, and visioning work. Keep in mind that I use "goal" here very loosely, since my system isn't really about achievement. 

### Goals and habits
These are heavily inspired by the [Full Focus planner system](https://fullfocus.co/). I use these templates to do some thinking ahead about what I'd like for myself in the future. I then include them into the priorities section in the yearly review file. The intention is to keep these visible every day, because I've found that any sense of urgency is lost if I don't see them regularly.

To use them within the review system, I state the goal in the title of the Obsidian file, and prepend it with "[current year] goal" or "[current year] habit."

### The visioning template
Every 3 years (or so) I like to set aside some time to take stock of where I am and where I'd like to go. You need to manually update any reference to the vision files to how you want it to work - that's not automated. Again, it's a place to do some separate thinking that I then bring into the yearly review file.

## Future iterations
I'm constantly fiddling with these review templates. 2023 was the first year I used this system. I was impressed at how I was able to take stock of my growth and progress, while also identifying places I still needed to build systems and guardrails. So if I figure out more systems and guardrails, I'll add them!
