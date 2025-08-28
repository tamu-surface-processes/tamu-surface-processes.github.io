---
permalink: /people/
title: "People"

postdocs:

graduatestudents:
  timko:
    name: Lena Timko
    img: /assets/images/people_images/LT_ProfilePhoto.jpg
    topic: Alluvial fan interaction
  zhi:
    name: Zhilin Shi
    img: /assets/images/people_images/bio-photo_zs.jpg
    topic: Delta compaction dynamics
    site: https://zshi1026.github.io/
  ujan:
    name: Ujan Dey
    img:  /assets/images/people_images/UD_Profile_Photo.jpg
    topic: River delta modelling


undergraduatestudents:
  almanza:
    name: Marcos Almanza
    img: /assets/images/people_images/MA_ProfilePhoto.jpg
    topic: Mapping grassland burn severity

# keep these in reverse-chronological order
formerstudents:
    lundeen:
      name: Elena Lundeen
      img: /assets/images/people_images/EL_ProfilePhoto.jpg
      topic: River-floodplain connectivity 
      degree: 2025, MS in Water Management and Hydrological Sciences
      aftergraduation: Fluvial Ecosystem Restoration group at Freese and Nichols
    cordova:
      name: Benjamin Cordova
      topic: Post-fire material movement
      img: /assets/images/people_images/BC_ProfilePhoto.jpg
      degree: 2025, BS in Geography
---


<!-- Note, the css that controls the display of the headshots is in _home.scss -->
<!-- Code here and in the css is based on: https://dmnfarrell.github.io/software/jekyll-galleries -->

## Faculty

![alt](/assets/images/people_images/moodie_2022_tamu_lowres.jpg){: width="250"}

**Dr. Andrew J. Moodie**\
[Google Scholar](https://scholar.google.com/citations?user=8wtbbNsAAAAJ)\
[Personal Website](https://andrewjmoodie.com)


## Postdocs

{% assign postdocs = page.postdocs %}
<div class ="image-gallery">
{% for person in postdocs %}
  <div class="box">
      <img src="{{ person[1]['img'] }}{{ name }} " alt="{{ name }}"  class="img-gallery" />
    <b>{{ person[1]['name'] }}</b><br>
    <i>{{ person[1]['topic'] }}</i><br>
    {% if person[1]['scholar'] %}
      <a href="{{ person[1]['scholar'] }}">Google Scholar</a><br>
    {% endif %}
    {% if person[1]['site'] %}
      <a href="{{ person[1]['site'] }}">Personal Website</a>
    {% endif %}
  </div>
{% endfor %}
</div>



## Graduate students

{% assign graduatestudents = page.graduatestudents %}
<div class ="image-gallery">
{% for person in graduatestudents %}
  <div class="box">
      <img src="{{ person[1]['img'] }}{{ name }} " alt="{{ name }}"  class="img-gallery" />
    <b>{{ person[1]['name'] }}</b><br>
    <i>{{ person[1]['topic'] }}</i><br>
    {% if person[1]['scholar'] %}
      <a href="{{ person[1]['scholar'] }}">Google Scholar</a><br>
    {% endif %}
    {% if person[1]['site'] %}
      <a href="{{ person[1]['site'] }}">Personal Website</a>
    {% endif %}
  </div>
{% endfor %}
</div>



## Undergraduate Students 

{% assign undergraduatestudents = page.undergraduatestudents %}
<div class ="image-gallery">
{% for person in undergraduatestudents %}
  <div class="box">
      <img src="{{ person[1]['img'] }}{{ name }} " alt="{{ name }}"  class="img-gallery" />
    <b>{{ person[1]['name'] }}</b><br>
    <i>{{ person[1]['topic'] }}</i><br>
    {% if person[1]['scholar'] %}
      <a href="{{ person[1]['scholar'] }}">Google Scholar</a><br>
    {% endif %}
    {% if person[1]['site'] %}
      <a href="{{ person[1]['site'] }}">Personal Website</a>
    {% endif %}
  </div>
{% endfor %}
</div>



## Former members
<!-- None yet. Will be a table of name, position, dates, and "now at" -->

{% assign formerstudents = page.formerstudents %}
<div class ="image-gallery">
{% for person in formerstudents %}
  <div class="box">
      <img src="{{ person[1]['img'] }}{{ name }} " alt="{{ name }}"  class="img-gallery" />
    <b>{{ person[1]['name'] }}</b><br>
    <i>{{ person[1]['topic'] }}</i><br>
    <ul>
      <li>{{ person[1]['degree'] }}</li>
      {% if person[1]['aftergraduation'] %}
        <li>After graduation: {{ person[1]['aftergraduation'] }}</li>
      {% endif %}
    </ul>
  </div>
{% endfor %}
</div>
