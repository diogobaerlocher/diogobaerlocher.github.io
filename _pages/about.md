---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

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
<p style="font-size:14px"><b> University of South Florida </b> <br/>
<span style="font-size:12px"> 
Intermediate Macroeconomics (undergraduate) <br/>
Economic Growth (undergraduate) <br/>
Macroeconomics II (graduate)  
</span>
</p>
<p style="font-size:14px"><b> University of Illinois </b> <br/>
<span style="font-size:12px"> 
Economic Growth (undergraduate)
</span>
</p>