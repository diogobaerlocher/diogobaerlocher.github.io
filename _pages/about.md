---
permalink: /
excerpt: "Associate Professor of Economics at the University of South Florida. Research on economic growth, public economics, and political economy, much of it on Brazil"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

 I'm an Associate Professor of Economics at the University of South Florida. My research asks why living standards differ across places, groups, and time, mostly through the lens of labor markets: how they respond to demographic change, how workers and activity reallocate across space, and how policy and politics shape them. Much of my work is set in Brazil and identified off historical episodes.

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
