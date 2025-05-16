---
layout: default
title: Students
---

# Students
This is a list of students in the course.

<ol>
  {% for student in site.students %}
    <li>
        <a href="{{ student.url }}">{{ student.name }}</a> ({{ student.class }})
    </li>
  {% endfor %}
</ol>
