{% assign data = include.data %}
<table class="asst-table">
<tr><th>Date</th><th>Topic</th><th>Intro &nbsp; &nbsp; &nbsp; &nbsp;</th><th>Worksheet</th></tr>
{% for ws in data.worksheets %} <!-- dummy comment to show comment syntax -->
<tr>
	<td>{{ ws.date }}</td>
	<td>{{ ws.topic }}</td>
	<td>
		<table class="inner">
		    <tr>
				{% if ws.iblank %}
			    <td><a href="{{ data.ihome }}/{{ ws.iblank }}">blank</a></td>
			    {% endif %}
			</tr>
			<tr>
 			    {% if ws.ifilled %}
			    <td><a href="{{ data.ihome }}/{{ ws.ifilled }}">filled</a></td>
			    {% endif %}
			</tr>
		</table>
		<div style="padding-bottom: 10px"></div>
	</td>
	<td>
		<table class="inner">
		    <tr>
				{% if ws.blank %}
			    <td><a href="{{ data.home }}/{{ ws.blank }}">blank</a></td>
			    {% endif %}
			</tr>
			<tr>
 			    {% if ws.filled %}
			    <td><a href="{{ data.home }}/{{ ws.filled }}">filled</a></td>
			    {% endif %}
			</tr>
		</table>
		<div style="padding-bottom: 10px"></div>
	</td>
</tr>
{% endfor %}
</table>
