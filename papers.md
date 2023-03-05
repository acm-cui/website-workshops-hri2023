---
layout: page
title: Accepted position papers

nav_text: Accepted papers
nav_position: 3
---

<table>
  <tr>
    <th>Author(s)</th>
    <th>Title</th>
  </tr>
  {% for entry in site.data.papers %}
  {% for paper in entry.papers %}
  <tr>
    <td></td>
    <td>{{paper.authors}}</td>
    <td><a href="{{ paper.pdf | absolute_url }}" title="View the PDF of {{ paper.title }}">{{ paper.title }}</a></td>
  </tr>
   {% endfor %}

{% endfor %}
</table>