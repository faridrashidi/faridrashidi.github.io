---
layout: default
title: About
---

<img style="border: 3px solid black; shape-outside: circle(); margin:0px 50px 0px 0px; border-radius: 50%; float: left; box-shadow:0 0 5px #828282;" src="https://www.gravatar.com/avatar/42125cfaaf0a859652acd4832533745d?s=2048"  width="180px" alt="me"/>

I am a predoctoral fellow at the [National Cancer Institute (NCI)](https://www.cancer.gov) [Center for Cancer Research (CCR)](https://ccr.cancer.gov) working in the [Cancer Data Science Laboratory (CDSL)](https://ccr.cancer.gov/cancer-data-science-laboratory) under supervision of [Dr. Cenk Sahinalp](https://algo-cancer.github.io). I am also a third-year Ph.D. student studying Computer Science at the [Indiana University Bloomington (IU)](https://www.indiana.edu). My main research focus is on [Tumor Heterogeneity](https://en.wikipedia.org/wiki/Tumour_heterogeneity) and Cancer Evolution. I completed [my Master’s thesis](http://library.sharif.ir/parvan/resource/444343/یادگیری-پیرایش-دگرسان-از-داده-های-توالی-یابی-آر--ان--ای/&from=search&&query=alternative%20splicing&count=20&execute=true) at the [Sharif University of Technology](http://www.en.sharif.edu) where I worked on learning of [Alternative Splicing](https://en.wikipedia.org/wiki/Alternative_splicing) problem, supervised by [Dr. Abolfazl Motahari](http://sharif.edu/~motahari/) and [Dr. Hamid Rabiee](http://sharif.edu/~rabiee/). I received my Bachelor’s degree from [Amirkabir University of Technology (Tehran Polytechnic)](https://aut.ac.ir/en) in Iran.

<br/>
Office: 2-6300, Building 10, [National Institutes of Health (NIH)](https://goo.gl/maps/XtuHbcXNd1tEC5us8)  
Email: frashidi AT iu DOT edu


<!-- ==================================================================================================== -->
<br/>
<h2 id="publications" style="margin-bottom:5px">Publications</h2>
<table style="width: 100%;">
    <tbody>
            {% for item in site.data.publications.publications %}
                <tr>
                    <td style="vertical-align:middle; border-bottom: 1px solid #e9e9e9;">
                        <a href="https://doi.org/{{ item.doi }}"><img src="/assets/{{ item.cover }}" style="max-height:100px; max-width:135px;"></a>
                    </td>
                    <td style="vertical-align:middle; border-bottom: 1px solid #e9e9e9;">
                        <div data-badge-popover="left" data-badge-type="donut" data-doi="{{ item.doi }}" data-hide-no-mentions="true" class="altmetric-embed"></div>
                    </td>
                    <td style="width:100%; vertical-align:middle; padding-left:15px;  padding-bottom:10px; border-bottom: 1px solid #e9e9e9;">
                        <p style="margin: 0">{{ item.title }}</p>
                        {% for btn in item.links %}
                            <a class="btn" href="{{ btn.url }}">{{ btn.title }}</a>
                        {% endfor %}
                    </td>
                </tr>
            {% endfor %}
    </tbody>
</table>


<!-- ==================================================================================================== -->
<br/>
<h2 id="software" style="margin-bottom:5px">Software</h2>
<table style="width: 100%;">
    <tbody>
        <tr>
            <td style="text-align:center; border-bottom: 1px solid #e9e9e9;">
                <a href="https://github.com/algo-cancer/PhISCS-BnB"><img src="/assets/logo.phiscsbnb.png" style="max-height:100px; max-width:135px;"></a>
            </td>
            <td style="width:100%; vertical-align:middle; padding-left:15px; padding-bottom:10px; border-bottom: 1px solid #e9e9e9;">
                <p><strong>PhISCS-BnB</strong></p>
                <p style="margin: 0">A fast tool for reconstructing the perfect tumor phylogeny using single-cell data via branch and bound algorithm</p>
                <a class="btn" href="https://github.com/algo-cancer/PhISCS-BnB">Code</a> <a class="github-button" href="https://github.com/algo-cancer/PhISCS-BnB" data-show-count="true" aria-label="Star algo-cancer/PhISCS-BnB on GitHub">Star</a> <a class="github-button" href="https://github.com/algo-cancer/PhISCS-BnB/fork" data-show-count="true" aria-label="Fork algo-cancer/PhISCS-BnB on GitHub">Fork</a>
            </td>
        </tr>
        <tr>
            <td style="text-align:center; border-bottom: 1px solid #e9e9e9;">
                <a href="https://github.com/sfu-compbio/PhISCS"><img src="/assets/logo.phiscs.png" style="max-height:100px; max-width:135px;"></a>
            </td>
            <td style="width:100%; vertical-align:middle; padding-left:15px; padding-bottom:10px; border-bottom: 1px solid #e9e9e9;">
                <p><strong>PhISCS</strong></p>
                <p style="margin: 0">A tool for sub-perfect tumor phylogeny reconstruction via integrative use of single-cell and bulk sequencing data, with later being an optional</p>
                <a class="btn" href="https://github.com/sfu-compbio/PhISCS">Code</a> <a class="github-button" href="https://github.com/sfu-compbio/PhISCS" data-show-count="true" aria-label="Star sfu-compbio/PhISCS on GitHub">Star</a> <a class="github-button" href="https://github.com/sfu-compbio/PhISCS/fork" data-show-count="true" aria-label="Fork sfu-compbio/PhISCS on GitHub">Fork</a>
            </td>
        </tr>
        <tr>
            <td style="text-align:center;">
                <a href="https://farid.one/kaggle-solutions/"><img src="/assets/logo.kaggle.png" style="max-height:100px; max-width:135px;"></a>
            </td>
            <td style="width:100%; vertical-align:middle; padding-left:15px; padding-bottom:10px;">
                <p><strong>Kaggle Solutions</strong></p>
                <p style="margin: 0">A searchable list of almost all available solutions and ideas shared by top performers in the past Kaggle competitions</p>
                <a class="btn" href="https://farid.one/kaggle-solutions/">Webpage</a> <a class="btn" href="https://github.com/faridrashidi/kaggle-solutions">Code</a> <span style="vertical-align:bottom"><a class="github-button" href="https://github.com/faridrashidi/kaggle-solutions" data-show-count="true" aria-label="Star faridrashidi/kaggle-solutions on GitHub">Star</a></span> <a class="github-button" href="https://github.com/faridrashidi/kaggle-solutions/fork" data-show-count="true" aria-label="Fork faridrashidi/kaggle-solutions on GitHub">Fork</a>
            </td>
        </tr>
    </tbody>
</table>
