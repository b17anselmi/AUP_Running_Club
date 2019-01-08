---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<body>
  <div >
    <img src="http://ac.aup.edu/~a98632/assets/ClubCover.png">
  </div>
<div>
  <br>
  <h1>Upcoming Events</h1>
  <div>
    <table style="width:100%">
      <tr>
        <th>Event</th>
        <th>Date</th>
        <th>Location</th>
        <th>Description</th>
      </tr>
      {% for post in site.categories.event limit:3 %}
      <tr>
        <td><h4>
          <a href="{{ post.url | relative_url }}">
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
</div>
</br>
<h1>Most Recent Blog Posts</h2>
{% for post in site.categories.blog limit:3 %}
  <article style="margin: 30px 10px 30px 10px;">
    <h2>
      <a href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    | {{ post.author }}
    <img style="margin: 10px 0px 10px 0px;" src="http://ac.aup.edu/~a98632/{{ post.image }}">
    {{ post.intro }} . . .
  </article>
{% endfor %}

<scriptsrc="https://code.jquery.com/jquery-3.3.1.slim.min.js"integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo"crossorigin="anonymous"></script><scriptsrc="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js"integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49"crossorigin="anonymous"></script><scriptsrc="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js"integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy"crossorigin="anonymous"></script></body>
