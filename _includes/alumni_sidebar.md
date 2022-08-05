
<b> FumaLab Alumni </b>

{% for alum in site.data.alumni %}
<hr>
<img class="img-fluid" src="{{alumn.image}}" {% if person.altimage %} onmouseover="this.src='{{alumn.altimage}}';" onmouseout="this.src='{{alumn.image}}';" {% endif %} alt="{{alumn.name}}"; width="365"; height="365"><br>
<div id = "{{alum.name}}" style="padding-top: 60px; margin-top: -60px;">
<p><strong>{{alum.name}}</strong> - <em>{{alum.position}}</em><br>
{% if alum.startdate %} {{alum.startdate}} - {% endif %}{{alum.enddate}} <br>
{% if alum.current %} Subsequent Position: {{alum.current}} {% endif %} </p>
</div> {% endfor %}

