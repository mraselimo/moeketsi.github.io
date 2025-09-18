---
layout: default

css: [ 'index' ]

icon: home
title: Home
---

<div class='pure-g'>

<div class='pure-u-1 pure-u-sm-1-2 pure-u-md-13-24 top-left'> 
{%- if site.author.photo -%}
  {%- if site.author.photo.local -%}
    {%- assign photo_url = site.baseurl | append: '/' | append: site.author.photo.local -%}
  {%- else -%}
    {%- assign photo_url = site.author.photo.remote -%}
  {%- endif %}
  <div>
    <img alt='{{ site.author.photo.alt }}' src='{{ photo_url }}'/>
  </div>
{% endif -%}
</div>

<div class='pure-u-1 pure-u-sm-1-2 pure-u-md-11-24 top-right' markdown='1'>

#### <i class='far fa-fw fa-sm fa-paper-plane'></i> Contact Me

<p class='indented' markdown='1'>
  <em>Office</em>:&nbsp; [John von Neumann Haus][Office], Berlin, Germany
  <br>
  <em>Email (Work)</em>:&nbsp; raselimm <i class='fas fa-fw fa-sm fa-at'></i> hu-berlin &bull; de
</p>

#### <i class='fas fa-fw fa-sm fa-glasses'></i> Technical Expertise

<p class='indented' markdown='1'>
  &#x2B29;&nbsp; Program Analysis and Testing 
  <br>
  &#x2B29;&nbsp; Automated Debugging
  <br>
  &#x2B29;&nbsp; Data Analysis 
</p>

</div>
<br>
<div class='pure-u-1 pure-u-md-13-24 bot-left' markdown='1'>

#### <i class='fas fa-fw fa-sm fa-user'></i> About Me

<div class='pure-g' style='text-align: justify; margin-top: -1em'>
<div id='bio' class='pure-u-1 pure-u-md-22-24' markdown='1'>

I am a <span class='color-medium-accent'>Postdoctoral Researcher</span>
working on Program Analysis and Testing with the [Software Engineering 
Research Group](https://www.informatik.hu-berlin.de/de/forschung/gebiete/se/) 
at [Humboldt-Universität zu Berlin][HU]
under the mentorship of [Prof. Dr. Lars Grunske](https://www.informatik.hu-berlin.de/de/Members/lars-grunske).

Before that, I earned a <span class='color-medium-accent'>Ph.D.</span> in [Computer Science][CS@SU] 
at [Stellenbosch University][SU], South Africa 🇿🇦 in 2023 under the 
supervision of [Prof. Bernd Fischer](https://bfischer.pages.cs.sun.ac.za/).

I am mostly interested in automated methods and developing tools that 
make software reliable mostly through automated testing and program
analysis.

</div>
</div>

</div>
<div class='pure-u-1 pure-u-md-11-24 bot-right' markdown='1'>

<h4>
  <i class='fas fa-fw fa-xs fa-rotate-90 fa-timeline'></i>
  Recent <a href='{{ site.baseurl }}/updates'>Updates</a>
</h4>

<div class='pure-g table'>
  {%- assign sorted_updates = site.updates | sort: 'date' | reverse -%}
  {%- for event in sorted_updates limit: 5 -%}
    {%- assign eventdate = event.date | date: '%s' -%}
    {%- assign highlight = event.highlight | default: site.default_highlight[event.type] -%}
    <div class='pure-u-1-8 pure-u-sm-1-12 pure-u-md-1-6 event-date'>
    {%- if event.end_date == null -%}
      {{- event.date | date: "%b" -}}<i>{{- event.date | date: "%y" -}}</i>
    {%- else -%}
      {%- assign year = event.date | date: "%y" -%}
      {%- assign end_year = event.end_date | date: "%y" -%}
      <div class='multimonth'>{{- event.end_date | date: "%b" -}}<i>{{- end_year -}}</i><br><b>&#8942;</b><br>
      {{- event.date | date: "%b" -}}<i>{{- year -}}</i>
      </div>
    {% endif %}
    </div>
    <div class='pure-u-1-12 event-icon color-more-faded {% if highlight %} color-{{ highlight }} {% endif %}'>
      <i class='fas fa-fw fa-{{ event.icon | default: site.default_icon[event.type] }}'></i>
    </div>
    <div class='pure-u-19-24 pure-u-sm-5-6 pure-u-md-3-4 event-description'>
      {% include tools/text_process.md data=event.headline %}
      {% if event.location != null -%}
        <div class='event-location'>(&hairsp;{{event.location}}&hairsp;)</div>
      {%- endif %}
    </div>
  {% endfor %}
</div>

</div>
</div>

{% include moeketsi_links.md %}

