---
layout: docs
title:  "schema.org Markup"
---


<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="{{ site.baseurl }}/docs">Docs</a></li>
    <li class="breadcrumb-item"><a href="{{ site.baseurl }}/docs/events">Events</a></li>
    <li class="breadcrumb-item active" aria-current="page">schema.org Markup</li>
  </ol>
</nav>

# schema.org Markup

Using one of several ways, webpages can be marked up so that the information can be programatically read.

[Their website](https://schema.org/) has more information.

There is a [special object for events](https://schema.org/Event).

It is always worth using this for any public events on webpages on your website - this information is used by many other applications.

## Problems with lack of an id

One problem is there is no commonly used id field. This is a problem when repeatedly fetching the latest information from a webpage.

For example:

1. A webpage has 4 different events on it.
2. A bot collects information about these events.
3. A week later, the bot wants to look for updated information.
4. The webpage now has 3 events; one event was cancelled and removed and another event has had a change of time and title.
5. The bot collects the new information.

At this stage, the bot has no way of linking the events it saw the first time to the events it saw the second time. This could be a problem if people expressed an interest in the events and the bot now wants to inform them of changes or cancellations.

There are sometimes other fields that can act as an id - for example, often a list of events will link out to one webpage per event. In this case you can maybe use the URL of the webpage for each individual event as an id; but that can always change too.

## Checking Markup

[Google has a tool for checking this.](https://search.google.com/structured-data/testing-tool)
