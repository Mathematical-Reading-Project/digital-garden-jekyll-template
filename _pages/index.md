---
layout: page
title: Home
id: home
permalink: /
---

## <small> Welcome to our (slighlty empty) </small> __Review Repository__ 

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Reading is fun! Reading maths can be very fun!

  The Mathematics Reading Project aims to create an online repository of book recommendations and reviews from the Oxford Community in order to promote good reads. We're particularly interested in books which have made you excited about a subject, books that have made you see a subject in a new and interesting way and books suitable for early years undergraduates and those with less advanced mathematical background. If you'd like to contribute then please follow this link and fill out a form! 
</p>




<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
