---
layout: default
title: About
---

I am a predoctoral fellow at the [National Cancer Institute (NCI)](https://www.cancer.gov) working in [Cancer Data Science Laboratory (CDSL)](https://ccr.cancer.gov/cancer-data-science-laboratory) under supervision of [Dr. Cenk Sahinalp](https://algo-cancer.github.io). I am also a Ph.D. student studying Computer Science at the [Indiana University Bloomington (IUB)](https://www.indiana.edu) since 2017. My main research focus is on [Tumor Heterogeneity](https://en.wikipedia.org/wiki/Tumour_heterogeneity) and Cancer Evolution using [Single-cell sequencing](https://en.wikipedia.org/wiki/Single_cell_sequencing) data. I completed [my Master’s thesis](http://library.sharif.ir/parvan/resource/444343/یادگیری-پیرایش-دگرسان-از-داده-های-توالی-یابی-آر--ان--ای/&from=search&&query=alternative%20splicing&count=20&execute=true) at the [Sharif University of Technology](http://www.en.sharif.edu) where I worked on learning of [Alternative Splicing](https://en.wikipedia.org/wiki/Alternative_splicing) problem, jointly supervised by [Dr. Abolfazl Motahari](http://sharif.edu/~motahari/) and [Dr. Hamid Rabiee](http://sharif.edu/~rabiee/). I received my Bachelor’s degree from [Amirkabir University of Technology (Tehran Polytechnic)](https://aut.ac.ir/en) in Iran.


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
          <a href="https://pubmed.ncbi.nlm.nih.gov/{{ item.pubmed }}"><img draggable="false" src="/assets/{{ item.cover }}" style="max-height:100px; max-width:135px; border-radius: 3%"></a>
        </td>
        <td style="width:100%; vertical-align:middle; padding-left:15px; padding-bottom:10px; {{ border }}">
          <p style="margin: 0">{{ item.title }}</p>
          <div class="altmetric-embed" data-badge-type="donut" data-doi="{{ item.doi }}" style="display:inline-block; width:30px; height:30px; vertical-align: -10px; margin-right:2px"></div>
          {% for btn in item.links %}
            <a class="btn" href="{{ btn.url }}">{{ btn.title }}</a>
          {% endfor %}
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
          <a href="{{ item.url }}"><img draggable="false" src="/assets/{{ item.cover }}" style="max-height:100px; max-width:135px;"></a>
        </td>
        <td style="width:100%; vertical-align:middle; padding-left:15px; padding-bottom:10px; {{ border }}">
          <p style="margin: 0">{{ item.title }}</p>
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
