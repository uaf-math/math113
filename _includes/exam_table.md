{% assign data = include.data %}
<table class="asst-table">
<tr><th>Semester</th>
    {% for e in data.exams %} <th>{{ e.name }}</th> {% endfor %}
</tr>
<tr>
	<td>{{ data.semester }}</td>
    {% for e in data.exams %}
	<td> 
		<a href="{{ data.home }}/{{ e.blank }}">blank</a><br>
		{% if e.solutions %}
		    <a href="{{ data.home }}/{{ e.solutions }}">solutions</a><br>
		{% endif %}
	</td>
	{% endfor %}
</tr>
</table>
