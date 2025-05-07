{% assign data = include.data %}
<table class="asst-table">
<tr><th>Due Date</th><th>Homework</th><th>Topic</th><th>Problems</th></tr>
{% for hw in data.homeworks %}
<tr>
  <td>{{ hw.due }}</td>
  <td>{{ hw.number }}</td>
  <td>{{ hw.topic }}</td>
  <td><a href="{{ data.home }}/{{ hw.problems }}">problems</a></td>
</tr>
{% endfor %}
</table>
