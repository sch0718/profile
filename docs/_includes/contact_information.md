{% if include.show_profile_url == false %}
  {% assign show_profile_url = false %}
{% else %}
  {% assign show_profile_url = include.show_profile_url | default: true %}
{% endif %}

# 📬 연락처

- +82 010 3397 0718
- sch0718@naver.com
{% if show_profile_url %}- https://sch0718.github.io/profile{% endif %}