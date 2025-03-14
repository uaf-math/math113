{% assign data = include.data %}
<table class="asst-table">
{% for exam in data.exams %}
<tr>
	<td> 
		<table class="inner">
		    <tr>
			    <td><b>{{ exam.name }}</b></td>
			</tr>
			{% if exam.date %}
			<tr>
			    <td> &nbsp; &nbsp; {{ exam.date }}</td>
			</tr>
			{% endif %}
			<tr>
			    <td>topics: {{ exam.topics }}</td>
			</tr>
		    {% if exam.cont %}
			<tr>
			    <td>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  {{ exam.cont }}</td>
			</tr>
			{% endif %}
		</table>
	</td>
	<td> 
		<table class="inner">
		  {% if exam.blank %}
		  <tr>
			    <td><a href="{{ data.home }}/{{ exam.blank }}">blank</a></td>
			</tr>
			{% endif %}
		  {% if exam.solutions %}
			<tr>
			    <td><a href="{{ data.home }}/{{ exam.solutions }}">solutions</a></td>
			</tr>
			{% endif %}
		</table>
		<div style="padding-bottom: 10px"></div>
	</td>
</tr>
{% endfor %}
</table>
