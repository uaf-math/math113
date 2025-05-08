{% assign data = include.data %}
<table class="asst-table">
<tr><th>Semester</th><th>Midterm I</th><th>Midterm II</th><th>Midterm III</th></tr>
<tr>
	<td>{{ data.semester }}</td>
    {% for m1 in data.midterm1 %}
	<td> 
		<a href="{{ data.home }}/{{ m1.blank }}">blank</a><br>
		<a href="{{ data.home }}/{{ m1.solutions }}">solutions</a><br>
	</td>
	{% endfor %}
    {% for m2 in data.midterm2 %}
	<td> 
		<a href="{{ data.home }}/{{ m2.blank }}">blank</a><br>
		<a href="{{ data.home }}/{{ m2.solutions }}">solutions</a><br>
	</td>
	{% endfor %}
    {% for m3 in data.midterm3 %}
	<td> 
		<a href="{{ data.home }}/{{ m3.blank }}">blank</a><br>
		<a href="{{ data.home }}/{{ m3.solutions }}">solutions</a><br>
	</td>
	{% endfor %}
</tr>
</table>
