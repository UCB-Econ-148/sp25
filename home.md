---
layout: page
title: Welcome!
nav_exclude: true
permalink: /
currWeekNumber: 1
---

# Data Science for Economists
{: .mb-2 }
UC Berkeley, Spring 2025
{: .mb-2 .fs-6 .text-grey-dk-000 }

[PollEV](https://pollev.com/ericvandusen){: .btn .btn-purple }
[Ed](https://edstem.org/){:target="_blank" .btn .btn-ed .mr-1 }
[Gradescope](https://www.gradescope.com/){:target="_blank" .btn .btn-gradescope .mr-1 }
[Lecture Recordings](https://kaltura.berkeley.edu/){:target="_blank" .btn .btn-recordings .mr-1} 
[Extenuating Circumstances](TODO){:target="_blank" .btn .btn-blue .mr-1 }
[Anonymous Feedback](TODO){:target="_blank" .btn .btn-feedback .mr-1 } 

{: .mb-2 }
**Instructor:** 
{: .mb-0 .fs-5 .text-grey-dk-000 }

<div>
{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
  <div class="role">
    {% for staffer in instructors %}
    {{ staffer }}
    {% endfor %}
  </div>
</div>

{: .mb-3 }
**Lecture:** Tuesday's and Thursday's, 2:00 - 3:30 PM, [Hearst Field Annex A1](https://dac.berkeley.edu/hearst-field-annex)       
{: .mb-0 .fs-5 .text-grey-dk-000 }

{: .mb-4 }        
**Office Hours:** TBD
{: .mb-0 .fs-5 .text-grey-dk-000 }

{: .highlight }
> Welcome to [Week {{page.currWeekNumber}}](#week-{{page.currWeekNumber}}) of Econ 148!

+ The schedule and dates listed below are tentative and may be subject to change. 
+ All announcements will be made via Ed.
+ The [Syllabus](./syllabus) contains a detailed explanation of how each course component will work this semester
+ If you plan to add late, make sure you contact the staff first to see if you can make up the missed assignments before officially adding the class. 

<a name="schedule"></a>
## Schedule
{% for module in site.modules %}
<a name="week-{{module.weekNumber}}"></a>
{{ module }}
{% endfor %}