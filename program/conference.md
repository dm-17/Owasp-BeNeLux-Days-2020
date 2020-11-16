---
title: Conference program
---

<div class="keynote-full">

	<ul>
	{% for speaker in site.data.conference %}
		{% if speaker.name %}
		<li>
    <p>
      <a name="{{speaker.name}}">
      <img style="background-image: url(/assets/images/conference/{{speaker.image | default:'owasp_logo.png'}});{{speaker.style}};"></a>
      <h2>{{speaker.title}} by {{speaker.name}}</h2>
      <p><em>{{speaker.day}}</em></p>
      <h4>Abstract:</h4>
        <p>{{speaker.abstract}}</p>
        <br>
      {% if speaker.bio %}
			<h4>Bio:</h4>
				<p>{{speaker.bio}}</p>
        <br>
      {% endif %}
    </p>
		</li>
		{% endif %}
	{% endfor %}
	</ul>
</div>
