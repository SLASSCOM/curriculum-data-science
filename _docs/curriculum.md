---
title: Course Curriculum
tags: 
 - curriculum
 - overview
 - course
description: Curriculum content
---

# Overview

Add some overview here.

<hr class="panel-line">

# Core Modules
Core modules description goes here.

{% assign folder = site.docs | where_exp: "post" , "post.path contains 'core'"%}
{% for post in folder %}
- <h6><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h6>
{% endfor %}

<hr class="panel-line">

# Elective Modules
{% assign folder = site.docs | where_exp: "post" , "post.path contains 'elective'"%}
{% for post in folder %}
- <h5><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h5>
{% endfor %}

<hr class="panel-line">

# Supplementary Modules
{% assign folder = site.docs | where_exp: "post" , "post.path contains 'supplementary'"%}
{% for post in folder %}
- <h5><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h5>
{% endfor %}
