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
    {% for post in site.categories.event %}
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


# Weekly Runs

Our weekly runs meet in Combes and take place along the Seine. We run for about 30 minutes, which is just enough time to get down to the west tip of  Île de la Cité if you run a sub 10 minute mile pace. Below you'll find our weekly plan for the current semester, as well as any special events we have happening.

<img src="/assets/view.jpg">

#### **Fall 2018**

Come join our weekly run on the Seine! We meet around 5:00-5:30 pm outside the athletics office on the 3rd floor of Combes, drop our bags, and head out. There are bathrooms on the 3rd floor if you need to change. We'll be back to Combes by 6:30 pm to collect our stuff.

<div style="float:right;">
  <iframe  src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2624.8102715584446!2d2.3038626156733715!3d48.86182820841861!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e66fd956d40469%3A0x93e97e03f4632aa7!2s6+Rue+du+Colonel+Combes%2C+75007+Paris!5e0!3m2!1sen!2sfr!4v1542573335769" width="400" height="300" frameborder="0" style="border:0" allowfullscreen></iframe>
</div>

We'll be out there and moving anywhere from 30-45 minutes. Everyone can go their own pace, in groups or solo, the point is to have a good time and a run (or even a walk) that makes you want to run again.

**What to bring:**

* Comfortable shoes/clothing
* Water (optional but recommended)
* Towel (optional)
* Watch and/or running app (optional)
* Headphones (optional)
* Friends (optional but highly recommended!)
* A smile! (required)


*Some things to note:*

There's limited space where we're going to lock up our stuff, so please only bring the essentials.

We'll be doing this every single week, rain or shine. If you can't make it that's totally fine, just know that I'll be there ready to run with anyone who wants to join me (unless otherwise announced).
