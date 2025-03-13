{% if include.show_portfolio == false %}
  {% assign show_portfolio = false %}
{% else %}
  {% assign show_portfolio = include.show_portfolio | default: site.show_portfolio %}
{% endif %}

### Hybrid-Cloud 개발 환경 자동화 구축 서비스 개발
- 기간: 2018.02 ~ 2018.06
- 개요: 소유하고 있는 Cloud 및 on-premises 환경을 모두 지원하는 개발 환경 self-service 시스템 개발
- 역할: Web Framework 개발, DB 설계, BE/FE 개발
- 개발 환경: AWS(EC2), Container, Linux, Embedded Tomcat
- 개발 언어: Java, JSP, javascript, CSS, shell script
- Data Platform/DBMS: MariaDB
- Framework/Tool: Spring Boot, JPA, MyBatis, Maven, Nexus, Jenkins, SonarQube, GitLab, Docker, jQuery
- 직무 경험 및 성과: 데브옵스 엔지니어들과 협업을 통한 서비스 개발 및 오픈, 클라우드 및 컨테이너 환경에서 개발 경험
{% if show_portfolio %}- 포트폴리오: [Metrom](./portfolio/metrom){:target="_blank"}{% endif %}

### 현대카드 빅데이터 검색 포털 시스템 (Shpere) 구축
- 기간: 2017.06 ~ 2018.01
- 개요: 빅데이터 분석 & Visualization, 데이터 검색 시스템 개발
- 역할: Project Tech Lead(업무 협의, BE/FE 개발 가이드 및 코드 리뷰), DB 설계, BE/FE 개발, 배치 쿼리 개발, SQL 튜닝
- 개발 환경: AWS(EC2), Container, Linux, Tomcat
- 개발 언어: Java, JSP, javascript, CSS, Scala, shell script
- Data Platform/DBMS: MySQL, MongoDB, Elasticsearch, Hadoop, Hive, Spark
- Framework/Tool: Spring Boot, JPA, MyBatis, Spring Batch, Maven, Nexus, Jenkins, SonarQube, Kibana, GitLab, Docker, Oozie