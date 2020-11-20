---
layout: post
title:  "How do we know what events people want to see on MeetYourNextMP?"
excerpt_separator: <!--more-->
tags: [MeetYourNextMP, Events]
---


	

MeetYourNextMP was a crowdsourced calendar of over 1000 independent events at the general election. This was to make 
these events easier to find so voters could go and question their candidates, and also to try and make more voters aware 
these events exist and are open to all.

When people came to the site, how did we know what events to show them? We asked people what their postcode was, and 
directed them to a page for each constituency. But what events did we show?

<!--more-->

Most hustings are pretty easy – they happen in the same constituency as the speakers are standing in and it’s easy to 
pick that up from the postcode of the venue.

However, there are many edge cases. In a densely populated area like London there are many constituencies close together, 
and events may feature speakers from several constituencies. Sometimes events may happen in another constituency 
altogether than the speakers may come from. This might happen in dense areas just due to which venues are available or 
in one extreme version of this, a regional TV station did hustings for many different seats all from the same central 
TV studio.

With event sites like this, it’s always a hard balance – the more information you ask for about an event, the more 
options you have to categorise it more usefully. But also, the more annoying it is to add an event and if you ask for 
too much information some people may stop adding them.

We decided to ask for the venue of the event and which candidates were speaking at the event. We put up a box with the 
names of the candidates in that seat for users to select from, but they could also press a button to search among all 
3,900 candidates standing. Many events had this information added, but not all.

With this information, we came up with a rule – a voter would be shown an event if it was in their seat or had a 
candidate from their seat speaking at it.

This meant if we had details of an event in a voter’s seat, but did not know who was speaking, we assumed it would be of 
interest to them and showed it to them. If a voter’s candidate was speaking at an event 20, 50 or 200 miles away, we 
showed that event too.

There were some edge cases where this didn’t work, of course.

There were a few cases where speakers were at events literally 500 miles away from their constituency. In this case, are 
voters still interested? Few will travel hundreds of miles just to hear a candidate speak, but they might want to know 
it happened. There may be online resources to look up. Some people who used the data filtered out events that were very 
far away, but we left these events on MeetYourNextMP.

For events that happened in a central TV studio, but concerned different constituencies, the people who lived near that 
TV Studio would presumably not be interested even though they would still be shown the event.

This is also, as you may be feeling if you’ve read this far, pretty dry and hard to explain to people. Certainly someone 
adding an event to the site just follows the prompts and mostly won’t read this amount of guidance.

We had cases where people added an event, but then tried to set the venue to be in another place than it actually was as 
they thought this was the way they could say the event was of interest to others. They would try and set the venue to be 
in “Edinburgh” instead of “Edinburgh South” if there were speakers from across Edinburgh standing. We had to correct this 
and look up or request extra information by hand.

Also, for regional TV and radio broadcasts it got more complicated – they would be only available to people in one 
region, but that region might contain many constituencies.

I considered if there was other ways to ask people for information that would help us show the event to interested 
people. Could we ask people to add an event then tell us which constituency it was about, bearing in mind they might 
have to select more than one? That sounds like a complex and annoying UI.

Could we just give up on constituencies, and look up the location of a postcode and show events within a certain mile 
radius? This is very imprecise and likely to annoy if it includes many events voters don’t think interest them because 
they feature speakers from different seats. Also, we didn’t always know the exact location of a venue. And I think it 
was good to have a separate distinct web page for each seat, as this is how the First Past The Post (FPTP) voting system 
works and it is how every other General Election website I’ve seen worked. It meant other sites could link to a good 
page on our site easily.

There was no easy answer to this problem, and this is quite a dry complex subject and thus blog post – thanks for 
reading so far! We think our system of having a page for each constituency and having a rule of showing events there 
if the event was in the constituency or featured a speaker from that constituency worked well almost all the time. 
Certainly we couldn’t think of a better one this time around, but maybe this will be discussed before the next time.

ps. Asking people what their postcode is, and directed them to a page for each constituency turns out to not always be 
fool proof – there are some postcodes that feature properties in 2 separate constituencies! This is indeed a tough issue.


_Written by [James Baster](https://www.jamesbaster.co.uk/)_

