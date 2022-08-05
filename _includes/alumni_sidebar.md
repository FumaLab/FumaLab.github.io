
<b><h1> FumaLab Alumni </h1> </b>

{% for alum in site.data.alumni %}
<hr>
<img class="img-fluid" src="{{alumn.image}}" {% if alumn.altimage %} onmouseover="this.src='{{alumn.altimage}}';" onmouseout="this.src='{{alumn.image}}';" {% endif %} alt="{{alumn.name}}"; width="100"; height="100"><br>
<div id = "{{alum.name}}" style="padding-top: 60px; margin-top: -60px;">
<p><strong>{{alum.name}}</strong> - <em>{{alum.position}}</em><br>
{% if alum.startdate %} {{alum.startdate}} - {% endif %}{{alum.enddate}} <br>
{% if alum.current %} Subsequent Position: {{alum.current}} {% endif %} </p>
</div> {% endfor %}

