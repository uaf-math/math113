---
layout: course-page
title: Math F113 Math in Society at UAF
---

### Homework Assignments

<div class="x-scroll">
<table class="asst-table">
<tr><th>Due Date</th><th>Homework</th><th>Topic</th><th>Problems</th></tr>
{% for c in site.data.homework %}
<tr valign="top">
  <td>
    {{ c.due }}
 </td>
  <td>{% for s in c.sections %}{{ s.number }}{% endfor %}</td>
  <td>
    {% for s in c.sections %}
      {{ s.topic }}
    {% endfor %}
 </td>
  <td>
    {% for s in c.sections %}
      <a href="assets/homework/S25/{{s.problems}}">problems</a>
    {% endfor %}
 </td>
</tr>
{% endfor %}
</table>
</div>
