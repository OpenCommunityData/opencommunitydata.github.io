---
layout: docs
title:  "Meetup.com"
---

<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="{{ site.baseurl }}/docs">Docs</a></li>
    <li class="breadcrumb-item"><a href="{{ site.baseurl }}/docs/events">Events</a></li>
    <li class="breadcrumb-item active" aria-current="page">Meetup.com</li>
  </ol>
</nav>

# Meetup.com

## API

While there is an API, you need to be a "Pro" member to apply for a API key now.

This effectively means that we can not consider their API as open in any way.

## iCal feeds

Meetup.com does have iCal feeds available, but they don't advertise them in their UI. This means you should treat such feeds as unsupported and fragile.

For an individual event page like:

    https://www.meetup.com/agile20reflect-meetup-group/events/276168360/

You can rewrite the URL as:

    https://www.meetup.com/agile20reflect-meetup-group/events/276168360/ical/x.ics


For a group page like:

    https://www.meetup.com/agile20reflect-meetup-group/
    
You can rewrite the URL as:

    https://www.meetup.com/agile20reflect-meetup-group/events/ical/ 


However in both cases the description is truncated (with a link back to the website included).

