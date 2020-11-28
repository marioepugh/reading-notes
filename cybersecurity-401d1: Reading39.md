Understanding SQL Injection, Identification and Prevention

What are SQL attacks? It is as simple as “I added a couple characters onto the end of a URL in my browser, now I’m committing felony unlawful access to a computer system.” 

Which is why we’re taking this point in time to point out that SQL Injection attacks are one of those situations where the outcome can be wildly disproportionate to the amount of effort that went into executing it.

Please approach practical aspects of this with the same seriousness as you would the new IT staff member telling you: “It’s just one command, how much damage could it possibly do?”

In particular, if you’re a sysadmin in any moderately sized organization, there are probably a half dozen internal applications that your company depends upon day in and day out which:

Are presumed to be internal, so security isn’t a big priority.
Were developed a decade or more ago when some security development practices weren’t as ingrained.
Will quite likely crash if you run even an “innocuous” SQL injection attack against them. For instance, you can often grind a database and web server to a halt simply by requesting all of the records in the database instead of the 1 record that the application page would typically load.

Standardized query language (SQL) is, in one form or another, still the dominant method of inserting, filtering and retrieving information from a database. Loads of SQL queries will be coursing through your web applications on almost every page load – regardless of if it’s a tiny toy website with a tiny SQLite file, or a popular ecommerce site with millions of visits per hour requiring a massive cluster of database servers from Enterprise Database Vendor of choice.

And so, armed with literally nothing but a web browser, some basic SQL knowledge and an internet connection, an attacker can exploit flaws in your web application – extracting user data, discovering or resetting credentials and using it as a launch point for deeper assaults on your network.

We’re going to get to work our way up to SQL injection attacks and the reason they are scarier than a clown who lives in a drainpipe. But in order to understand injection/vulnerabilities, we need to take a step back and review that basic SQL knowledge first, which you may not have needed until this point in your role as a sysadmin.

One of the really remarkable things about SQL is that the basics of the language haven’t changed much since it was first invented in the early 1970s. While some of the more esoteric commands differ between the major database vendors and open source options, the basics are the same across almost everything.

With that in mind, if you want to follow along with the steps below, here’s an SQLite database of all the data referenced in this article – as well as a link to DB Browser for SQLite – a cross platform, open source query tool to use with the example file.
