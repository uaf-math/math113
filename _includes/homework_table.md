{% assign data = include.data %}
<table class="asst-table">
{% for homework in data.homework %}
<tr>
  <td><b>{{ homework.due }}</b><br>
  <td><b>{{ homework.number }}</b><br>
  <td>
		<table class="inner">
		  <tr>
          <td><b>{{ homework.topic }}</b><br>
			    <td><a href="{{ data.home }}/{{ hw.problems }}">problems</a></td>
		  </tr>
		</table>
	</td>           
</tr>
{% endfor %}
</table>
