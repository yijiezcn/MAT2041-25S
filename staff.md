---
layout: page
title: Teaching Staff
description: A listing of all the course staff members.
---

# Staff

Feel free to reach out if you have any.
## Instructor

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}

## Teaching Assistants

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

## USTF

{% assign USTF = site.staffers | where: 'role', 'USTF' %}
{% for staffer in USTF %}
{{ staffer }}
{% endfor %}
