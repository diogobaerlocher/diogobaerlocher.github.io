---
permalink: /
excerpt: "Associate Professor of Economics at the University of South Florida. Research on economic growth, public economics, and political economy, much of it on Brazil."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

I'm an Associate Professor of Economics at the University of South Florida. My research asks why living standards differ across places, groups, and time, and I come at that question from both the aggregate and the individual side. The proximate causes I study include labor market composition, the spatial reallocation of people and activity, and demographic change, including women's entry into the labor force and the formation of racial identity. The fundamental causes I approach through political behavior, treating how individuals vote and respond to their governments as the micro foundation of the institutions within which those forces operate. Much of this work is set in Brazil and identified off historical episodes.

<span class="title"> Working Papers </span>
{% for post in site.projects reversed %}
  {% include archive-single.html %}
{% endfor %}
<br/>
<span class="title"> Peer-Reviewed Publications </span>
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
<br/>
<span class="title"> Peer-Reviewed Publications (Portuguese) </span>
{% for post in site.portuguese reversed %}
  {% include archive-single.html %}
{% endfor %}
<br/>
<span class="title"> Teaching </span>
<p style="font-size:1rem"><b> University of South Florida </b> <br/>
<span style="font-size:0.875rem"> 
Intermediate Macroeconomics (undergraduate) <br/>
Economic Growth (undergraduate) <br/>
Macroeconomics II (graduate)  
</span>
</p>
<p style="font-size:1rem"><b> University of Illinois </b> <br/>
<span style="font-size:0.875rem"> 
Economic Growth (undergraduate)
</span>
</p>
