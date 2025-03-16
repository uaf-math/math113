---
layout: course-page
title: Math F113 Math in Society at UAF
---

### Worksheets

<div class="x-scroll">
<table class="asst-table">
<tr><th>Worksheet</th><th>Date</th><th> </th><th> </th></tr>
{% for c in site.data.worksheets %}
<tr valign="top">
  <td>
    {{ c.worksheet }}
 </td>
  <td>{% for s in c.sections %}{{ s.date }}{% endfor %}</td>
  <td>
    {% for s in c.sections %}
       <a href="assets/worksheets/S25/{{s.blank}}">blank</a>
    {% endfor %}
 </td>
  <td>
    {% for s in c.sections %}
      <a href="assets/worksheets/S25/{{s.filled}}">filled</a>
    {% endfor %}
 </td>
</tr>
{% endfor %}
</table>
</div>
