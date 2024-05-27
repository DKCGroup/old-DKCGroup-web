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
<div class="col-sm-2">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/KaichenDong.jpg" class="img-responsive" width="80%" style="float: left" />
</div>
<div class="col-sm-5">
  <h3>Kaichen Dong</h3>
  <i>Assistant Professor, started Nov. 2022 
  <br>email: <dkc22@sz.tsinghua.edu.cn></i>
  <h4> Professional Experience </h4>
  <ul style="overflow: hidden">
  <li> 2024/01 – Now: Director, Intelligent Passive Thermal Control Center (IPTCC), Research Institute of Tsinghua University in Shenzhen </li>
  <li> 2023/09 – Now: Deputy Director,<a href="https://cdh.sigs.tsinghua.edu.cn/main.htm"> Center of Double Helix (CDH) </a>, Tsinghua Shenzhen International Graduate School, Tsinghua University </li>
  <li> 2023/02 – Now: Assistant Professor, Tsinghua-Berkeley Shenzhen Institute (TBSI), Institute of Data and Information (iDI), Tsinghua Shenzhen International Graduate School, Tsinghua University </li>
  <li> 2022/11 – 2023/02: Assistant Professor, Tsinghua-Berkeley Shenzhen Institute (TBSI), Tsinghua Shenzhen International Graduate School, Tsinghua University </li>
  <li> 2019/03 – 2022/09: Affiliate in Materials Science Division, Lawrence Berkeley National Laboratory. Supervisor: Professor Junqiao Wu </li>
  <li> 2019/02 – 2022/09: Postdoctoral Researcher in Materials Science and Engineering, University of California, Berkeley. Advisors: Professor Junqiao Wu, Professor Jie Yao </li>
  <li> 2017/10 – 2019/01: Research Associate in Precision Instrument, Tsinghua University. Supervisor: Professor Zheng You </li>
  </ul>
</div>

<div class="col-sm-5">
  
  <h4> Education Background </h4>
  <ul style="overflow: hidden">
  <li> 2015/07 – 2016/12: Affiliate in Materials Science Division, Lawrence Berkeley National Laboratory. Supervisor: Professor Junqiao Wu </li>
  <li> 2014/12 – 2016/12: Visiting Ph.D. student in Materials Science and Engineering, University of California, Berkeley. Advisors: Professor Junqiao Wu, Professor Jie Yao </li>
  <li> 2012/09 – 2017/10: Ph.D. in Precision Instrument, Tsinghua University. Advisor: Professor Zheng You </li>
  <li> 2008/08 – 2012/07: B.E. in Precision Instrument, Tsinghua University</li>
  </ul>

  <h4> Awards & Honors: </h4>
  <ul style="overflow: hidden">
  <li>2024/03, <a href="https://piers.org/awards/young-scientist-award.html">PIERS Young Scientist Award</a></li>
  <li>2023/12, Chief Scientist of National Key R&D (Young Scientist) Program of China</li>
  <li>2022/12, Shenzhen Pengcheng Peacock Plan (Class B)</li>
  <li>2022/10, National Science Foundation of China (NSFC) Early-Career Award</li>
  <li>2022/06, <a href="https://www.technologyreview.com/innovator/kaichen-dong">MIT Technology Review Top 35 Innovators Under 35 (TR35, Global List)</a></li>
  <li>2018/11, National Excellent Doctoral Dissertation in the Field of Measurement, Control and Instrument by China Instrument and Control Society (ranking 1st)</li>
  <li>2018/07, Excellent Doctoral Dissertation of Tsinghua University</li>
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
{% for member in site.data.undergrads %}

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
