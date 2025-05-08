{% assign data = include.data %}
<table class="asst-table">
<tr><th>Topic</th><th>Description</th></tr>
{% for ws in data.projectS25 %} <!-- dummy comment to show comment syntax -->
<tr>
	<td>{{ ws.topic }}</td>
	<td>{{ ws.pdf }}</td>
		</table>
		<div style="padding-bottom: 10px"></div>
	</td>
</tr>
{% endfor %}
</table>
