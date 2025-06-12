---
layout: default
title: Students
---

# Students

## Class 1C
<ol>
  {% for student in site.students %}
    {% if student.class contains "1C" %}
        <li>
            {{ student.class }} <a href="{{ student.url }}">{{ student.name }}</a>  [<a href="{{ student.website }}" target="_blank">{{ student.website }}</a>]
        </li>
    {% endif %}
  {% endfor %}
</ol>

## Class 1D
<ol>
  {% for student in site.students %}
    {% if student.class contains "1D" %}
        <li>
            {{ student.class }} <a href="{{ student.url }}">{{ student.name }}</a>  [<a href="{{ student.website }}" target="_blank">{{ student.website }}</a>]
        </li>
    {% endif %}
  {% endfor %}
</ol>

## Class 1E
<ol>
  {% for student in site.students %}
    {% if student.class contains "1E" %}
        <li>
            {{ student.class }} <a href="{{ student.url }}">{{ student.name }}</a>  [<a href="{{ student.website }}" target="_blank">{{ student.website }}</a>]
        </li>
    {% endif %}
  {% endfor %}
</ol>
