---
title: 신춘호 Profile
show_portfolio: false
---

{% include contact_information.md show_profile_url=false %}

{% include about_me.md %}

{% assign expand_yogiyo = page.expand_yogiyo | site.expand_projects.yogiyo %}
{% assign expand_megazonecloud = page.expand_megazonecloud | site.expand_projects.megazonecloud %}
{% assign expand_codepost = page.expand_codepost | site.expand_projects.codepost %}
{% assign expand_ensystem_2016 = page.expand_ensystem_2016 | site.expand_projects.ensystem_2016 %}
{% assign expand_ydata = page.expand_ydata | site.expand_projects.ydata %}
{% assign expand_ensystem_2015 = page.expand_ensystem_2015 | site.expand_projects.ensystem_2015 %}
{% assign expand_4csoft = page.expand_4csoft | site.expand_projects.4csoft %}
{% assign expand_nextweb = page.expand_nextweb | site.expand_projects.nextweb %}
{% assign expand_swotsoft = page.expand_swotsoft | site.expand_projects.swotsoft %}
{% assign expand_topnwise = page.expand_topnwise | site.expand_projects.topnwise %}
{% include work_experience.md 
    expand_yogiyo=expand_yogiyo
    expand_megazonecloud=expand_megazonecloud
    expand_codepost=expand_codepost
    expand_ensystem_2016=expand_ensystem_2016
    expand_ydata=expand_ydata
    expand_ensystem_2015=expand_ensystem_2015
    expand_4csoft=expand_4csoft
    expand_nextweb=expand_nextweb
    expand_swotsoft=expand_swotsoft
    expand_topnwise=expand_topnwise
%}

{% include skills.md %}

{% include education.md %}

{% include military_service.md %}

{% include certifications.md %}
