
<b><h3> FumaLab Alumni </h3> </b>

{% for alum in site.data.alumni %}
<hr>
<div id = "{{alum.name}}" style="padding-top: 60px; margin-top: -60px;">
<p><strong>{{alum.name}}</strong> - <em>{{alum.position}}</em><br>
{% if alum.startdate %} {{alum.startdate}} - {% endif %}{{alum.enddate}} <br>
{% if alum.current %} Subsequent Position: {{alum.current}} {% endif %} </p>
</div> {% endfor %}

