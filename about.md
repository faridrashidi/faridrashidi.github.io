---
layout: default
title: About
---

<table style="width:100%; margin-left: auto; margin-right: auto;">
  <tr>
    <td width="60%">
      <img style="margin:0px 10px 0px 0px; border-radius: 5%; box-shadow:0 0 5px #828282; float:right" src="https://www.gravatar.com/avatar/42125cfaaf0a859652acd4832533745d?s=2048" width="220px"/>
    </td>
    <td width="40%">
      {% include social.html %}
    </td>
  </tr>
</table>

<p style="text-align: center;">
  Office: 2-6300, Building 10, <a href="https://goo.gl/maps/XtuHbcXNd1tEC5us8">National Institutes of Health (NIH)</a>
  <br> Email: frashidi AT iu DOT edu
</p>

<br/>

I am a predoctoral fellow at the [National Cancer Institute (NCI)](https://www.cancer.gov) [Center for Cancer Research (CCR)](https://ccr.cancer.gov) working in the [Cancer Data Science Laboratory (CDSL)](https://ccr.cancer.gov/cancer-data-science-laboratory) under supervision of [Dr. Cenk Sahinalp](https://algo-cancer.github.io). I am also a third-year Ph.D. student studying Computer Science at the [Indiana University Bloomington (IUB)](https://www.indiana.edu). My main research focus is on [Tumor Heterogeneity](https://en.wikipedia.org/wiki/Tumour_heterogeneity) and Cancer Evolution. I completed [my Master’s thesis](http://library.sharif.ir/parvan/resource/444343/یادگیری-پیرایش-دگرسان-از-داده-های-توالی-یابی-آر--ان--ای/&from=search&&query=alternative%20splicing&count=20&execute=true) at the [Sharif University of Technology](http://www.en.sharif.edu) where I worked on learning of [Alternative Splicing](https://en.wikipedia.org/wiki/Alternative_splicing) problem, supervised by [Dr. Abolfazl Motahari](http://sharif.edu/~motahari/) and [Dr. Hamid Rabiee](http://sharif.edu/~rabiee/). I received my Bachelor’s degree from [Amirkabir University of Technology (Tehran Polytechnic)](https://aut.ac.ir/en) in Iran.

<br/><br/>
{% include title-bar.html title="Publications" %}
<table style="width: 100%;">
  <tbody>
    {% for item in site.data.publications.publications %}
      {% if item.number == '1' %}
        {% assign border = "" %}
      {% else %}
        {% assign border = "border-bottom: 1px solid #e9e9e9;" %}
      {% endif %}
      <tr>
        <td style="vertical-align:middle; {{ border }}">
          <a href="https://pubmed.ncbi.nlm.nih.gov/{{ item.pubmed }}"><img src="/assets/{{ item.cover }}" style="max-height:100px; max-width:135px;"></a>
        </td>
        <!-- <td style="vertical-align:middle; {{ border }}">
          <div data-badge-type="donut" data-doi="{{ item.doi }}" data-hide-no-mentions="true" class="altmetric-embed"></div>
        </td> -->
        <td style="width:100%; vertical-align:middle; padding-left:15px;  padding-bottom:10px; {{ border }}">
          <p style="margin: 0">{{ item.title }}</p>
          {% for btn in item.links %}
            <a class="btn" href="{{ btn.url }}">{{ btn.title }}</a>
          {% endfor %}
          <div class="altmetric-embed" data-badge-type="1" data-doi="{{ item.doi }}"></div>
        </td>
      </tr>
    {% endfor %}
  </tbody>
</table>
<br/><br/>


{% include title-bar.html title="Software" %}
<table style="width: 100%;">
  <tbody>
    {% for item in site.data.software.software %}
      {% if item.number == '1' %}
        {% assign border = "" %}
      {% else %}
        {% assign border = "border-bottom: 1px solid #e9e9e9;" %}
      {% endif %}
      <tr>
        <td style="text-align:center; {{ border }}">
          <a href="{{ item.url }}"><img src="/assets/{{ item.cover }}" style="max-height:100px; max-width:135px;"></a>
        </td>
        <td style="width:100%; vertical-align:middle; padding-left:15px; padding-bottom:10px; {{ border }}">
          <p><strong>{{ item.title }}</strong></p>
          <p style="margin: 0">{{ item.subtitle }}</p>
          {% for btn in item.links %}
            <a class="btn" href="{{ btn.url }}">{{ btn.title }}</a>
          {% endfor %}
          <a class="github-button" href="https://github.com/{{ item.id }}" data-show-count="true" aria-label="Star {{ item.id }} on GitHub">Star</a> <a class="github-button" href="https://github.com/{{ item.id }}/fork" data-show-count="true" aria-label="Fork {{ item.id }} on GitHub">Fork</a>
        </td>
      </tr>
    {% endfor %}
  </tbody>
</table>
<br/><br/>
