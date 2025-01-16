---
layout: page
title: Staff
description: A listing of all the course staff members.
nav_order: 4
---

# Staff 🧑‍🏫

<!-- See [this post](https://edstem.org/us/courses/34369/discussion/) on Ed for the most up-to-date office hours schedule and Zoom links. -->

## Instructor

Email the instructor with any questions about the class.

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
<div class="role">
  {% for staffer in instructors %}
  {{ staffer }}
  {% endfor %}
</div>

## Staff

{% assign staff = site.staffers | where: 'role', 'Staff' %}
<div class="role">
  {% for staffer in staff %}
  {{ staffer }}
  {% endfor %}
</div>