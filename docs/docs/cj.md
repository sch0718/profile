# 요기요 데이터 시각화 서비스 개발 및 운영/고도화
- 기간: 2020.04 ~ 2024.09
- 1차 구축:
    - 개요: 요기요의 가게(이름, 주소, 상품, 리뷰 등), 주문(주문일시, 결제정보, 가게/고객 정보 등), 배달(배달방법, 배달시간, 라이더 등), 고객(이름, 나이, 성별, 리뷰 등), 지역(지역특성, 인구 등) 등의 데이터를 총 망라하여 기본정보 및 분석된 정보를 시각화하여 내부(마케팅 활용, 가게 영업등) or 외부에 제공하는 서비스 개발
    - 역할: 아키텍처 설계, GKE(GCP/k8s) 환경에 인프라 구성 및 CI/CD 프로세스 확립 및 파이프라인 개발, BE/FE 개발
사용자 그룹 간 비교 및 Target 데이터 추출 기능 개발
- 2차 고도화
    - 개요: 요기요 App 내 사용자 주문 시점의 가게 랭킹 시뮬레이션 기능 개발, 고객의 리뷰 내용을 ML 모델로 분석하여 어뷰징 및 욕설 감지, 리뷰 내 맛/식감 분류 및 분석 기능 개발
    - 역할: BE/FE 개발, ML 모델 서빙 및 관련 API 개발 및 시각화
- 3차 리뉴얼:
    - 개요: 데이터 시각화 서비스 전체 리뉴얼, 기존 기능 및 데이터 이관 및 현행화, 표준 카탈로그 플랫폼 데이터 교정 기능 개발, 사용자 Profile 및 Segment 데이터를 이용한 
    - 역할: Project Tech Lead(프로젝트 관리 및 업무 협의, BE/FE 개발 가이드 및 코드 리뷰), 아키텍처 설계, DB 설계, 컨텐츠 기획
- 개발 환경: GCP, k8s(GKE), Container, Linux
- 개발 언어: Python, React, typescript, CSS(LESS), shell script
- Data Platform/DBMS: BigQuery, PostgreSQL, Elasticsearch, Redis
- Framework/Tool: FastAPI, Flask, SQLAlchemy, poetry, pandas, NextJS, Helm, skaffold, Terraform, ArgoCD, Datadog, Kibana, Github, Bitbucket, Github Action, Tekton, Docker, Airflow, Jupyter Notebook, EChart, Leaflet, Material UI, Ant Design, bokeh

# 요기요 사용자 행동 로그 관리, 로그 수집 및 정합성 체크, 로그 분석 통계 서비스 구축 및 운영, 고도화
- 기간: 2023.01 ~ 2024.09
- 개요: 요기요의 다양한 App(배달, 라이더, 사장님 등)에서 발생하는 사용자 행동 로그를 정의하고, 정의된 대로 전송되는지 실시간(debug app only)으로 체크하고, 전송된 로그를 적재하여 비즈니스 분석에 활용할 데이터의 품질을 높이기 위한 시스템 개발
- 역할: Project Tech Lead(프로젝트 관리 및 업무 협의, BE/FE 개발 가이드 및 코드 리뷰), 아키텍처 설계, DB 설계, 컨텐츠 기획
- 개발 환경: GCP, k8s(GKE), Container, Linux
- 개발 언어: Python, React, typescript, CSS(LESS), shell script
- Data Platform/DBMS: BigQuery, PostgreSQL, GCP Pub/Sub, Redis
- Framework/Tool: FastAPI, SQLAlchemy, poetry, pandas, NextJS, Helm, skaffold, Terraform, ArgoCD, Datadog, Github, Github Action, Docker, Airflow, Jupyter Notebook, EChart, Material UI

# 요기요 MLOps Platform 구축 및 배달 시간 예측 모델 실시간 서빙 서비스 개발
- 기간: 2022.02 ~ 2023.03
- 개요: 요기요 App내 주문 전/후 배달 예상 시간을 예측하기 위한 ML 모델을 서빙하고, 지속적인 모델의 예측 정확도를 유지하기 위한 지속적 학습(Continuous Training) 환경을 제공, 가게별 배달 시간 설정 및 제공 방식을 관리하는 시스템 개발
- 역할: Project Tech Lead(프로젝트 관리 및 업무 협의, FE 개발 가이드 및 코드 리뷰), 아키텍처 설계, DB 설계, BE 개발, ML 모델 서빙을 위한 CI/CD/CT 파이프라인 구축 참여, 성능 모니터링 및 개선
- 개발 환경: GCP, k8s(GKE), Container, Linux
- 개발 언어: Python, React, typescript, CSS(LESS), shell script
- Data Platform/DBMS: BigQuery, PostgreSQL, Kafka(Confluent Cloud), Redis
- Framework/Tool: FastAPI, poetry, pandas, NextJS, Helm, skaffold, Terraform, ArgoCD, Datadog, Github, Github Action, Docker, Airflow, Jupyter Notebook, EChart, Material UI

# 메가존클라우드 DevOps 서비스 개발
- 기간: 2018.10 ~ 2019.10
- 개요: Project Management Service의 개발 티켓으로부터 간단한 설정 및 결재 프로세스를 통해 개발/운영 환경 Provisioning 및 CI/CD 파이프라인을 template 기반으로 소유한 Cloud 환경에 빠르고 쉽게 배포할 수 있는 기능을 제공
- 역할: 아키텍처 설계, DB 설계, BE/FE 개발, open source 솔루션 활용 및 커스터마이즈
- 개발 환경: AWS(Fargate), Container, Linux, Embedded Tomcat
- 개발 언어: Java, Vue, javascript, CSS, shell script
- Data Platform/DBMS: MariaDB, Redis, RabbitMQ
- Framework/Tool: Spring Cloud, JPA, MyBatis, Concourse CI, Maven, Nexus, SonarQube, GitLab, Docker

# 코드포스트 Hybrid-Cloud 개발 환경 자동화 구축 서비스 개발
- 기간: 2018.02 ~ 2018.06
- 개요: 소유하고 있는 Cloud 및 on-premises 환경을 모두 지원하는 개발 환경 self-service 시스템 개발
- 역할: Web Framework 개발, DB 설계, BE/FE 개발
- 개발 환경: AWS(EC2), Container, Linux, Embedded Tomcat
- 개발 언어: Java, JSP, javascript, CSS, shell script
- Data Platform/DBMS: MariaDB
- Framework/Tool: Spring Boot, JPA, MyBatis, Maven, Nexus, Jenkins, SonarQube, GitLab, Docker, jQuery경험

# 현대카드 빅데이터 검색 포털 시스템 (Shpere) 구축
- 기간: 2017.06 ~ 2018.01
- 개요: 빅데이터 분석 & Visualization, 데이터 검색 시스템 개발
- 역할: Project Tech Lead(업무 협의, BE/FE 개발 가이드 및 코드 리뷰), DB 설계, BE/FE 개발, 배치 쿼리 개발, SQL 튜닝
- 개발 환경: AWS(EC2), Container, Linux, Tomcat
- 개발 언어: Java, JSP, javascript, CSS, Scala, shell script
- Data Platform/DBMS: MySQL, MongoDB, Elasticsearch, Hadoop, Hive, Spark
- Framework/Tool: Spring Boot, JPA, MyBatis, Spring Batch, Maven, Nexus, Jenkins, SonarQube, Kibana, GitLab, Docker, Oozie

# SK Planet Data White Book / Cleat QR 신규 개발 및 BIS 시스템 모니터링
- 기간: 2016.04 ~ 2017.02
- 개요: SK Planet에서 운영하고 있는 서비스들의 데이터를 통합하여 데이터 플랫폼을 구축하고, 데이터 플랫폼을 통해 데이터를 분석하고 시각화하는 시스템 개발
- 역할: DB 설계, BE/FE 개발, 배치 쿼리 개발
- 개발 환경: Linux, Tomcat
- 개발 언어: Java, JSP, javascript, CSS, shell script
- Data Platform/DBMS: Oracle, MySQL, MongoDB, Hadoop, Hive
- Framework/Tool: Spring Boot, MyBatis, Spring Batch, Maven, Jenkins, SVN, Oozie, jQuery

# 삼성 에스원 안심모바일 홈페이지 개편 및 다이렉트몰 구축, MVNO 서비스 연동
- 기간: 2015.10 ~ 2016.02
- 개요: 다이렉트몰 개발 및 MVNO(Mobile Virtual Network Operator) 연동(KT, SKT)
- 역할: DB 설계, BE/FE 개발, 통신사 MVNO 서비스 연동
- 개발 환경: Windows, JEUS
- 개발 언어: Java, JSP, javascript, CSS
- Data Platform/DBMS: Oracle
- Framework/Tool: Spring, MyBatis, Maven, Jenkins, SVN, jQuery

# SKT T-Life 추천 시스템 구축 및 운영
- 기간: 2015.06 ~ 2015.07
- 개요: Web Log 기반 추천 시스템 관리 기능 개발 및 추천 Logic 검증 기능 개발
- 역할: BE/FE 개발
- 개발 환경: Linux, Tomcat
- 개발 언어: Java, JSP, javascript, CSS, shell script
- Data Platform/DBMS: Oracle, Hadoop, Hive
- Framework/Tool: Spring, MyBatis, Maven, Jenkins, SVN, Oozie, jQuery