{% if include.show_projects_expand == false %}
  {% assign show_projects_expand = false %}
{% else %}
  {% assign show_projects_expand = include.show_projects_expand | default: site.show_projects_expand %}
{% endif %}
{% assign expand_yogiyo = include.expand_yogiyo | default: site.expand_projects.yogiyo %}
{% assign expand_megazonecloud = include.expand_megazonecloud | default: site.expand_projects.megazonecloud %}
{% assign expand_codepost = include.expand_codepost | default: site.expand_projects.codepost %}
{% assign expand_ensystem_2016 = include.expand_ensystem_2016 | default: site.expand_projects.ensystem_2016 %}
{% assign expand_ydata = include.expand_ydata | default: site.expand_projects.ydata %}
{% assign expand_ensystem_2015 = include.expand_ensystem_2015 | default: site.expand_projects.ensystem_2015 %}
{% assign expand_4csoft = include.expand_4csoft | default: site.expand_projects.4csoft %}
{% assign expand_nextweb = include.expand_nextweb | default: site.expand_projects.nextweb %}
{% assign expand_swotsoft = include.expand_swotsoft | default: site.expand_projects.swotsoft %}
{% assign expand_topnwise = include.expand_topnwise | default: site.expand_projects.topnwise %}
# 💻 경력사항

## 주식회사 위대한상상

> 재직 기간: 2020.03.30 ~ 2024.10.01  
> 고용 형태: 정규직  
> 팀/직책: Data Service팀 / 팀장  
> 역할: Team Leader, 팀/프로젝트 관리, 데이터 플랫폼 구축 및 운영, 아키텍처/DB 설계, Backend 개발, Frontend 개발, CI/CD 파이프라인 개발

{% if show_projects_expand %}
<details markdown="1"{% if expand_yogiyo %} open="true"{% endif %}>
<summary>📋 프로젝트 상세 보기</summary>
{% endif %}

{% include_relative projects/yogiyo.md %}

{% if show_projects_expand %}
</details>
{% endif %}

---

## 메가존클라우드 주식회사

> 재직 기간: 2018.09.05 ~ 2020.03.28  
> 고용 형태: 정규직  
> 팀/직책: DevOps팀 / 팀원  
> 역할: 데브옵스 서비스 개발 및 운영, 아키텍처/DB 설계, Backend 개발, Frontend 개발  

{% if show_projects_expand %}
<details markdown="1"{% if expand_megazonecloud %} open="true"{% endif %}>
<summary>📋 프로젝트 상세 보기</summary>
{% endif %}

{% include_relative projects/megazonecloud.md %}

{% if show_projects_expand %}
</details>
{% endif %}

---

## 코드포스트 주식회사

> 재직 기간: 2017.04.10 ~ 2018.08.01
> 고용 형태: 정규직  
> 팀/직책: 서비스 개발팀 / 팀원  
> 역할: 데브옵스 서비스 개발 및 운영, 프로젝트 수행, DB 설계, Backend 개발, Frontend 개발  

{% if show_projects_expand %}
<details markdown="1"{% if expand_codepost %} open="true"{% endif %}>
<summary>📋 프로젝트 상세 보기</summary>
{% endif %}

{% include_relative projects/codepost.md %}

{% if show_projects_expand %}
</details>
{% endif %}

---

## 엔시스템(NSYSTEM)

> 재직 기간: 2016.04.04 ~ 2017.02.28  
> 고용 형태: 프리랜서  
> 팀/직급: 빅데이터사업부 / 과장  
> 역할: 프로젝트 수행  

{% if show_projects_expand %}
<details markdown="1"{% if include.expand_ensystem_2016 %} open="true"{% endif %}>
<summary>📋 프로젝트 상세 보기</summary>
{% endif %}

{% include_relative projects/ensystem_2016.md %}

{% if show_projects_expand %}
</details>
{% endif %}

---

## 와이데이터서비스

> 재직 기간: 2015.09.19 ~ 2016.02.03  
> 고용 형태: 프리랜서  
> 팀/직급: 시스템사업부 / 과장  
> 역할: 프로젝트 수행  

{% if show_projects_expand %}
<details markdown="1"{% if include.expand_ydata %} open="true"{% endif %}>
<summary>📋 프로젝트 상세 보기</summary>
{% endif %}

{% include_relative projects/ydata.md %}

{% if show_projects_expand %}
</details>
{% endif %}

---

## 엔시스템(NSYSTEM)

> 재직 기간: 2015.06.01 ~ 2015.07.31  
> 고용 형태: 프리랜서  
> 팀/직급: 빅데이터사업부 / 과장  
> 역할: 프로젝트 수행  

{% if show_projects_expand %}
<details markdown="1"{% if include.expand_ensystem_2015 %} open="true"{% endif %}>
<summary>📋 프로젝트 상세 보기</summary>
{% endif %}

{% include_relative projects/ensystem_2015.md %}

{% if show_projects_expand %}
</details>
{% endif %}

---

## 주식회사 포씨소프트

> 재직 기간: 2013.08.05 ~ 2015.04.11  
> 고용 형태: 정규직  
> 팀/직급: 개발팀 / 과장  
> 역할: Project Tech Lead, DB 설계, Backend 개발, Frontend 개발  

{% if show_projects_expand %}
<details markdown="1"{% if include.expand_4csoft %} open="true"{% endif %}>
<summary>📋 프로젝트 상세 보기</summary>
{% endif %}

{% include_relative projects/4csoft.md %}

{% if show_projects_expand %}
</details>
{% endif %}

---

## (주) 넥스트웹

> 재직 기간: 2010.04.05 ~ 2013.06.15  
> 고용 형태: 정규직  
> 팀/직급: 개발팀, 연구소 / 대리  
> 역할: Project Tech Lead, 개인화 통계/추천 솔루션 개발, DB 설계, Backend 개발, Frontend 개발  

{% if show_projects_expand %}
<details markdown="1"{% if include.expand_nextweb %} open="true"{% endif %}>
<summary>📋 프로젝트 상세 보기</summary>
{% endif %}

{% include_relative projects/nextweb.md %}

{% if show_projects_expand %}
</details>
{% endif %}

---

## (주) 스왓소프트

> 재직 기간: 2008.08.01 ~ 2010.02.26  
> 고용 형태: 정규직  
> 팀/직급: 개발팀 / 대리  
> 역할: Project Tech Lead, 그룹웨어/전자결재 솔루션 개발, DB 설계, Backend 개발, Frontend 개발  

{% if show_projects_expand %}
<details markdown="1"{% if include.expand_swotsoft %} open="true" {% endif %}>
<summary>📋 프로젝트 상세 보기</summary>
{% endif %}

{% include_relative projects/swotsoft.md %}

{% if show_projects_expand %}
</details>
{% endif %}

---

## 탑앤와이즈(주)

> 재직 기간: 2007.03.01 ~ 2008.07.05 (2006.11 ~ 2007.02 인턴)  
> 고용 형태: 정규직  
> 팀/직급: 개발팀, 솔루션연구소 / 대리  
> 역할: 포털 솔루션 개발, Backend 개발, Frontend 개발  

{% if show_projects_expand %}
<details markdown="1"{% if include.expand_topnwise %} open="true"{% endif %}>
<summary>📋 프로젝트 상세 보기</summary>
{% endif %}

{% include_relative projects/topnwise.md %}

{% if show_projects_expand %}
</details>
{% endif %}

---