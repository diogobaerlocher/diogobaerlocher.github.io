---
permalink: /
excerpt: "Associate Professor of Economics at the University of South Florida. Research in macroeconomic development, public economics, and political economy."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

I am an Associate Professor in the [Department of Economics](https://www.usf.edu/arts-sciences/departments/economics/) at the University of South Florida. My research combines growth theory with reduced-form empirical work, studying how history, demography, and public institutions shape long-run development. Much of it focuses on Brazil.

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
