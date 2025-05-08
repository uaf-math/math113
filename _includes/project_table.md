{% assign data = include.data %}
<table class="asst-table">
<tr><th>Topic</th><th></th></tr>
{% for c in data.projects %}
<tr>
  <td>{{ c.topic }}</td>
  <td><a href="{{ data.home }}/{{ c.pdf }}">description</a></td>
</tr>
{% endfor %}
</table>
