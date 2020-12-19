---
layout: home
title: Home
<!-- nav_exclude: true -->
nav_order: 0
seo:
  type: Course
  name: Reproducibility DeCal
---

# {{ site.tagline }}
{: .mb-2 }
{{ site.description }}
{: .fs-6 .fw-300 }

{% assign instructors = site.staffers | where: 'role', 'Instructor' %} {% for staffer in instructors %} {{ staffer }} {% endfor %}

### Psych 198 Spring 2021
- Course meetings: Wednesdays 7-8:30 PM Pacific Time starting Wednesday, February 3rd, 2021.
	- Synchronous via Zoom
	- Each class meeting consists of short lectures, discussion of topics from readings, and the occasional live code demonstrations and hands-on exercise.
	- Navigate to [Course Information](about.md) page for more detail on the course.

{% if site.announcements %}
{{ site.announcements.last }}
[All Announcements](announcements.md){: .btn .btn-outline .fs-3 }
{% endif %}

{% for module in site.modules %}
{{ module }}
{% endfor %}