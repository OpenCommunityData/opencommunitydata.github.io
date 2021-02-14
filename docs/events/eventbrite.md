---
layout: docs
title:  "Eventbrite"
---


<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="{{ site.baseurl }}/docs">Docs</a></li>
    <li class="breadcrumb-item"><a href="{{ site.baseurl }}/docs/events">Events</a></li>
    <li class="breadcrumb-item active" aria-current="page">Eventbrite</li>
  </ol>
</nav>

# Eventbrite

## iCal feeds

Eventbrite does have iCal feeds available, but they don't advertise them in their UI. This means you should treat such feeds as unsupported and fragile.

For an individual event page like:

    https://www.eventbrite.co.uk/e/comedy-crossing-the-animal-crossing-standup-comedy-show-tickets-129098692665

You can rewrite the URL as:

    http://www.eventbrite.co.uk/calendar.ics?eid=129098692665&calendar=ical

However the description is not included, and merely links back to the website.

For an organiser page like:

    https://www.eventbrite.co.uk/o/the-national-archives-2226699547
    
We don't know a way to get an iCal feed.
