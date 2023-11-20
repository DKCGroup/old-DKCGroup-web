---
title: "Dong Lab -- Team"
layout: gridlay
excerpt: "Dong Lab -- Team members"
sitemap: false
permalink: /team/
---

# Group Members

 **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see vacancies)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**

## Principle Investigator
<div class="row">
<div class="col-sm-6">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/KaichenDong.jpg" class="img-responsive" width="25%" style="float: left" />
  <h3>Kaichen Dong</h3>
  <i>Assistant Professor, started Nov. 2022 
  <br>email: <dkc22@sz.tsinghua.edu.cn></i>
  <h4> Professional Experience </h4>
  <ul style="overflow: hidden">
  <li> Kaichen also holds positions as the deputy director at the <a href="https://cdh.sigs.tsinghua.edu.cn/main.htm
"> center of Double Helix (CDH) </a> and the assistant professor at the <a href="https://www.sigs.tsinghua.edu.cn/en/2023/0315/c1303a59844/page.htm
"> institute of Data and Information (iDI) </a>  </li> 
  <li> Postdoc Researcher at UC Berkeley, Department of Materials Science and Engineering with Prof. Junqiao Wu and Prof. Jie Yao </li>
  <li> Postdoc affiliate at Lawrence Berkeley National Laboratory with Prof. Junqiao Wu </li>
  <li> Research associate at Tsinghua University, Department of Precision Instrument with Prof. Zheng You </li>
  </ul>

</div>

<div class="col-sm-6">
  
  <h4> Education Background </h4>
  <ul style="overflow: hidden">
  <li> Ph.D at Tsinghua University, Department of Precision Instrument with Prof. Zheng You</li> 
  <li> Visiting Ph.D. student at UC Berkeley, Department of Materials Science and Engineering, with Prof. Junqiao Wu and Prof Jie Yao </li>
  <li> B.E at Tsinghua University, Department of Precision Instrument. </li>
  </ul>

  <h4> Awards & Honors: </h4>
  <ul style="overflow: hidden">
  <li> 2022, Shenzhen Pengcheng Peacock Plan (Class-B)</li> 
  <li> 2022, National Early-Career Award </li>
  <li> 2022, <a href="https://www.technologyreview.com/innovator/kaichen-dong"> MIT Technology Review’s Global 35 Innovators Under 35 </a> </li>
  <li> 2018, National Excellent Doctoral Dissertation Award in the field of Measurement, Control and Instrument from the China Instrument and Control Society </li>
  <li> 2018, Excellent Ph.D. Thesis, Tsinghua University </li>
  </ul>
</div>
</div>

## Administrative Assistant

<div class="row">
<div class="col-sm-6">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/yuemengwang.jpeg" class="img-responsive" width="25%" style="float: left" />
  <h3>Yuemeng(Yona) Wang</h3>
  <i>Administrative assistant, started June 2023.
  <br>email: <wangyuemeng@sz.tsinghua.edu.cn></i>
</div>
</div>

## Ph.D/Master Students
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h3>{{ member.name }}</h3>
  <i>{{ member.info }} 
  <br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Undergraduate Students

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h3>{{ member.name }}</h3>
  <i>{{ member.info }} 
  <br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

 {% if member.number_educ == 6 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

   {% if member.number_educ == 7 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}
  
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
