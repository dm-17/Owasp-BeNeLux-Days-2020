---
title: Conference program
---

<div class="keynote-full">

	<ul>
	{% for speaker in site.data.conference %}
		{% if speaker.name %}
		<li>
    <p>
      <img style="background-image: url(/assets/images/conference/{{speaker.image}});{{speaker.style}};">
      <h2>{{speaker.title}} by {{speaker.name}}</h2>
      <h4>Abstract:</h4>
        <p>{{speaker.abstract}}</p>
        <br>
			<h4>Bio:</h4>
				<p>{{speaker.bio}}</p>
        <br>
    </p>



		</li>
		{% endif %}
	{% endfor %}
	</ul>
</div>
