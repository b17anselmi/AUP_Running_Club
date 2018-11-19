---
layout: page
title: Events
permalink: /events/
---
Here you'll find all the information about our events throughout the semester.

## Upcoming Events

<div>
  <table style="width:100%">
    <tr>
      <th>Event</th>
      <th>Date</th>
      <th>Description</th>
      <th>Location</th>
    </tr>
    {% for post in site.categories.event limit:5 %}
    <tr>
      <td><h4>
        <a href="{{ post.url }}">
          {{ post.title }}
        </a>
      </h4></td>
      <td><time datetime="{{ post.actualDate | actualDate: "%Y-%m-%d" }}">{{ post.actualDate | date_to_long_string }}</time></td>
      <td><a href="{{locationLink}}"> {{ post.locationName }}</a></td>
      <td><p>{{post.description}}</p></td>
    </tr>
  {% endfor %}
  </table>
</div>

&nbsp;


## Weekly Runs

Our weekly runs meet in Combes and take place along the Seine. We run for about 30 minutes, which is just enough time to get down to the west tip of  Île de la Cité if you run a sub 10 minute mile pace. Take a look at our current semester plan below.



{% for plan in site.categories.plan limit:1 %}
  <h3> <a href="{{plan.url}}">{{plan.title}}</a></h3>
  {{plan.description}}
{% endfor %}
<img src="/assets/route.png">
