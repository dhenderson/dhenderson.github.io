---
title: Democratizing data in your nonprofit
published: true
layout: post
date: 2016-05-31
tags:
- nonprofit
- data
- R
- dashboard
---

It wasn't long ago that data existed at the outskirts of the nonprofit psyche. In the last few years however, *interest* in social sector data has spiked, even if [capacity has not kept pace][do-good-data-2015].

A few pioneering nonprofits are making big bets on the transformative potential of data by hiring [Chief Data Officers][chief-data-officer], like my employer the [Family Independence Initiative][fii] (FII). For data to truly be transformative however, it cannot be the exclusive domain of those with "data" somewhere in their job descriptions.

Fundamentally, data analytics is about *listening in aggregate*, listening to those you serve, about what is working, and what is not. Everyone in your organization needs to listen. Therefore, everyone in your organization needs access to data.

When I joined FII there was a clear line between the "data people", who had access to our analytics, and everyone else. Like most nonprofits, when someone outside the data team needed to access the data, a request would come in to the data team and someone would perform some analysis and report back.

When I joined FII one of my initial focuses was making sure *everyone* in the organization had access to our data. To achieve data access ubiquity, I built a series of internal facing data dashboards that empower staff to explore and extract the data they need via a web-browser on their own.

**Shiny dashboards to the rescue**

I conduct my data analytics with the popular [statistical programming language R][R]. R provides tremendous power to split and explore data as well as build any range of models from econometrics through machine-learning. 

In order to get the power of the R language into the browser I developed FII's data dashboards using a server framework called [Shiny Server][shiny]. I taught a surprisingly well attended [session at this year's Do Good Data conference][shiny-session] on building Shiny dashboards, and am open to writing more technical posts on using Shiny in nonprofits if there's interest.

Shiny has been a godsend, enabling me to spin up new dashboards practically at will. Our data dashboards are organized by topic. For example, we have dashboards for demographics, financials, education, health, etc.

Each dashboard allows staff to input custom report parameters, such as the time interval, specific demographics characteristics, and variables the staff member wants to explore. Below is a screen shot of our financials dashboard.

![Financials dashboard][financials-dashboard]

The beauty of Shiny is that you have the full power of R underneath, so your dashboards are only limited by your imagination (and of course R skills). Below is another example of one of our dashboards, this one showing educational outcomes by age ranges:

![Education dashboard][education-dashboard]

I'm heartened that the social sector is recognizing that data is important, but now begins the more difficult work of putting that realization to practice. The first step I believe is getting data out of the "data dungeon" and into the hands of everyone in the organization. After all, if data analysis is really listening in aggregate, who in your organization wouldn't be aided by listening more closely?

[shiny-session]: http://www.dogooddata.com/agenda/session/115179
[shiny]: https://www.rstudio.com/products/shiny/shiny-server/
[R]: https://www.r-project.org
[do-good-data-2015]: http://fullcontactphilanthropy.com/2015/05/04/what-i-learned-about-the-state-of-analytics-in-the-social-sector-at-the-do-good-data-conference/
[financials-dashboard]: /assets/images/2016/05/financials.png
[education-dashboard]: /assets/images/2016/05/education.png
[chief-data-officer]: http://fullcontactphilanthropy.com/2014/04/28/hire-a-chief-data-officer/
[fii]: http://www.fii.org