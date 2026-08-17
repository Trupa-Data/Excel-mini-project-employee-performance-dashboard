## Employee Performance Dashboard (Excel)

This one started as a practice exercise and turned into one of my favorite mini-projects. I took a raw HR dataset — the kind with duplicate rows, blank cells, inconsistent naming, all the usual mess — and turned it into a one-page Excel dashboard that actually tells you something useful about how departments and employees are performing.

## The problem I was solving

Raw HR spreadsheets are usually unusable as-is. Someone in leadership wants to know "which department is underperforming" or "who are our top people," and the honest answer is buried in a few thousand rows nobody's going to scroll through. I wanted to practice the exact workflow an HR or ops analyst would go through: clean the data, calculate the right metrics, and present it in a way a non-technical manager could glance at and understand in ten seconds.

## What I actually did

First came the cleanup — duplicate records removed, missing values handled, columns standardized so formulas wouldn't choke on inconsistent formatting. From there I built out the metrics using AVERAGEIF, COUNTIF, IF, and VLOOKUP to calculate performance scores by department and role. Then I summarized everything with pivot tables before moving into the dashboard layer, where I used charts, slicers, and conditional formatting to make the whole thing interactive instead of just a static report.

## What's on the dashboard

A bar chart comparing average performance score across departments — Sales came out on top, followed by Marketing, Operations, and IT
A pie chart breaking down headcount by role (Analyst, Engineer, Manager)
Summary cards for overall average performance (2.8), total headcount (120), and the top individual performer


## What the numbers actually showed

Sales and Marketing had the strongest average performance scores of any department. Operations had the biggest headcount of the group but didn't score as well on average — which is exactly the kind of gap a dashboard like this is supposed to surface, since it's not obvious from the raw data until you break it out this way. It's a small dataset, so I'm not claiming statistical rigor here — more that this is the kind of pattern a real HR dashboard would need to flag for someone to dig into further.

## Tools

Excel — data cleaning, formulas, pivot tables, dashboard build
Conditional formatting — for flagging performance tiers at a glance
Slicers — so the dashboard stays interactive instead of static
Folder structure
├── data/        # Raw and cleaned HR datasets
├── dashboard/   # The Excel dashboard file (.xlsx)
├── visuals/     # Screenshots of the dashboard
└── README.md

## Why I built this

I wanted a project that wasn't just "here's a chart" but actually walked through a realistic ask — someone hands you messy HR data and expects a usable summary back. That's the workflow I tried to replicate here, formulas and all.

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/1a3bd514-1fab-40bc-acf4-be2d64c2e1f0" />


