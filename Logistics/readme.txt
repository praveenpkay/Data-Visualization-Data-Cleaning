Dataset: https://lnkd.in/gDJQSMz
Dashboard: https://lnkd.in/gvz2BjU

There's something about cleaning data that is oddly satisfying.
While the colorful #BI dashboards always steal the thunder, little is
spoken about the cleaning, processing that fundamentally went in.

Here, I've got a real-time logistics dataset, whose quality is not at its best,
it has got wrong, duplicate, fraudulent entries, missing values, repetition of fields, etc.
in fact, most practical datasets tend to have these issues.

Pandas-Profiling as a preliminary analysis conveys
pertinent information/characteristics of each and every field.

But data cleaning might be time-consuming as the dimension increases,
so it is of utmost importance that one must focus only on the relevant fields
for relevant problem statements.

Cascaded Lambda functions with filter, map, apply makes the whole preprocessing kinda fun.
Here's the preprocessing function that gives a refined output for my dashboard.
I've tried to reduce any kind of field processing inside #tableau to reduce its load.
All that's left now is to visualize and bring out the KPIs.