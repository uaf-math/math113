{% assign data = include.data %}
{% comment %}
I've commented out the Due Date header and due date slots here so that in the future we can just re-use this page regardless of semester. But if you want to put them back you can uncomment things.
{% endcomment %}
<table class="asst-table">
<tr>{% comment %}<th>Due Date</th>{% endcomment %}<th>Homework</th><th>Topic</th><th>Problems</th></tr>
{% for hw in data.homeworks %}
<tr>
  {% comment %}<td>{{ hw.due }}</td>{% endcomment %}
  <td>{{ hw.number }}</td>
  <td>{{ hw.topic }}</td>
  <td><a href="{{ data.home }}/{{ hw.problems }}">problems</a></td>
</tr>
{% endfor %}
</table>
