---
layout: course-page
title: Homework
---

### Homework Problems

<div class="x-scroll">
<table class="asst-table">
<tr><th>Due Date</th><th>Homework</th><th>Topic</th><th>Problems</th></tr>
{% for c in site.data.homework_s2025 %}
<tr valign="top">
  <td>
    {{ c.due }}
  </td>
  <td>
    {{ c.number }}
  </td>
  <td>
    {{ c.topic }}
  </td>
  <td>
    <a href="{{ c.problems }}">problem set</a> 
  </td>
</tr>
{% endfor %}
</table>
</div>
