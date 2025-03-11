{% assign show_portfolio = include.show_portfolio | default: site.show_portfolio %}

### 요기요 데이터 시각화 서비스 리뉴얼
- 기간: 2023.04 ~ 2024.09
- 개요: 데이터 시각화 서비스 전체 리뉴얼, 기존 기능 및 데이터 이관 및 현행화, 표준 카탈로그 플랫폼 데이터 교정 기능 개발, 사용자 Profile 및 Segment 데이터를 이용한 사용자 그룹 간 비교 및 Target 데이터 추출 기능 개발
- 역할: Project Tech Lead(프로젝트 관리 및 업무 협의, BE/FE 개발 가이드 및 코드 리뷰), 아키텍처 설계, DB 설계, 컨텐츠 기획
- 개발 환경: GCP, k8s(GKE), Container, Linux
- 개발 언어: Python, React, typescript, CSS(LESS), shell script
- Data Platform/DBMS: BigQuery, PostgreSQL, Elasticsearch, Redis
- Framework/Tool: FastAPI, SQLAlchemy, poetry, pandas, NextJS, Helm, skaffold, Terraform, ArgoCD, Datadog, Kibana, Github, Github Action, Docker, Airflow, Jupyter Notebook, EChart, Leaflet, Material UI
- 직무 경험 및 성과: 요기요 임직원 1300명 중 **MAU 300명 이상**이 사용하는 서비스를 **기획, 설계, 개발, 운영 등 전체 과정에 참여** 하였고, 당시 요기요 서비스의 핵심 기능인 할인 랭킹을 위한 메뉴 분류 체계의 Human In the Loop 방식을 통한 데이터 교정 기능 개발하여 **서비스 품질 향상에 기여**

### 사용자 행동 로그 관리, 로그 수집 및 정합성 체크, 로그 분석 통계 서비스 구축 및 운영, 고도화
- 기간: 2023.01 ~ 2024.09
- 개요: 요기요의 다양한 App(배달, 라이더, 사장님 등)에서 발생하는 사용자 행동 로그를 정의하고, 정의된 대로 전송되는지 실시간(debug app only)으로 체크하고, 전송된 로그를 적재하여 비즈니스 분석에 활용할 데이터의 품질을 높이기 위한 시스템 개발
- 역할: Project Tech Lead(프로젝트 관리 및 업무 협의, BE/FE 개발 가이드 및 코드 리뷰), 아키텍처 설계, DB 설계, 컨텐츠 기획
- 개발 환경: GCP, k8s(GKE), Container, Linux
- 개발 언어: Python, React, typescript, CSS(LESS), shell script
- Data Platform/DBMS: BigQuery, PostgreSQL, GCP Pub/Sub, Redis
- Framework/Tool: FastAPI, SQLAlchemy, poetry, pandas, NextJS, Helm, skaffold, Terraform, ArgoCD, Datadog, Github, Github Action, Docker, Airflow, Jupyter Notebook, EChart, Material UI
- 직무 경험 및 성과: **대용량의 데이터(로그, 일 1억건 이상)를 처리할 수 있는 아키텍처 설계**, **로그의 품질 향상(60%~70% → 95% 이상)**을 통한 데이터 분석 신뢰도 향상 및 서비스 품질 개선에 기여
{% if show_portfolio %}
- 포트폴리오: [I.Log.Yo](./portfolio/ilogyo)
{% endif %}

### 배달 시간 예측 모델 실시간 서빙 서비스 구축
- 기간: 2022.09 ~ 2023.03
- 개요: 요기요 App내 주문 전/후 배달 예상 시간을 예측하기 위한 ML 모델을 서빙하고, 지속적인 모델의 예측 정확도를 유지하기 위한 지속적 학습(Continuous Training) 환경을 제공, 가게별 배달 시간 설정 및 제공 방식을 관리하는 시스템 개발
- 역할: Project Tech Lead(프로젝트 관리 및 업무 협의, FE 개발 가이드 및 코드 리뷰), 아키텍처 설계, DB 설계, BE 개발, ML 모델 서빙을 위한 CI/CD/CT 파이프라인 구축 참여, 성능 모니터링 및 개선
- 개발 환경: GCP, k8s(GKE), Container, Linux
- 개발 언어: Python, React, typescript, CSS(LESS), shell script
- Data Platform/DBMS: BigQuery, PostgreSQL, Kafka(Confluent Cloud), Redis
- Framework/Tool: FastAPI, poetry, pandas, NextJS, Helm, skaffold, Terraform, ArgoCD, Datadog, Github, Github Action, Docker, Airflow, Jupyter Notebook, EChart, Material UI
- 직무 경험 및 성과: **트래픽의 변화에 따라 실시간 컨테이너 오케스트레이션 및 대규모 트래픽을 소화할 수 있는 형태의 아키텍처 설계**, **모니터링을 통한 지속적인 성능 개선 및 최적화(피크타임 기준 평균 latency 100ms → 20ms)**, ML 모델의 개발 및 서빙을 위한 전체 과정을 직·간접 경험, 지리 정보 관련 데이터 처리 및 개발

### 요기요 데이터 시각화 서비스 고도화
- 기간: 2020.11 ~ 2022.08
- 개요: 요기요 App 내 사용자 주문 시점의 가게 랭킹 시뮬레이션 기능 개발, 고객의 리뷰 내용을 ML 모델로 분석하여 어뷰징 및 욕설 감지, 리뷰 내 맛/식감 분류 및 분석 기능 개발
- 역할: BE/FE 개발, ML 모델 서빙 및 관련 API 개발 및 데이터 시각화 화면 개발
- 개발 환경: GCP, k8s(GKE), Container, Linux
- 개발 언어: Python, React, typescript, CSS(LESS), shell script
- Data Platform/DBMS: BigQuery, PostgreSQL, Elasticsearch, Redis
- Framework/Tool: Flask, SQLAlchemy, poetry, pandas, Helm, skaffold, Kibana, Bitbucket, Docker, Jupyter Notebook, EChart, Leaflet, Ant Design
- 직무 경험 및 성과: **AI/ML 개발/서비스 환경 구축 및 API 서빙**, 가게 랭킹 시뮬레이션을 통한 추천 서비스 개선에 기여, 리뷰 어뷰징 및 욕설 감지 서비스를 통한 CS 업무 효율 증대에 기여
{% if show_portfolio %}
- 포트폴리오: [YoDa](./portfolio/yoda)
{% endif %}

### 요기요 데이터 시각화 서비스 구축
- 기간: 2020.04 ~ 2020.09
- 개요: 요기요의 가게(이름, 주소, 상품, 리뷰 등), 주문(주문일시, 결제정보, 가게/고객 정보 등), 배달(배달방법, 배달시간, 라이더 등), 고객(이름, 나이, 성별, 리뷰 등), 지역(지역특성, 인구 등) 등의 데이터를 총 망라하여 기본정보 및 분석된 정보를 시각화하여 내부(마케팅 활용, 가게 영업등) or 외부에 제공하는 서비스 개발
- 역할: 아키텍처 설계, GKE(GCP/k8s) 환경에 인프라 구성 및 CI/CD 프로세스 확립 및 파이프라인 개발, BE/FE 개발
- 개발 환경: GCP, k8s(GKE), Container, Linux
- 개발 언어: Python, React, typescript, CSS(LESS), shell script
- Data Platform/DBMS: BigQuery, PostgreSQL, Elasticsearch, Redis
- Framework/Tool: Flask, SQLAlchemy, poetry, pandas, Helm, skaffold, Tekton, Kibana, Bitbucket, Docker, Jupyter Notebook, EChart, Leaflet, Ant Design, bokeh
- 직무 경험 및 성과: redash를 커스터마이즈한 BI 서비스가 AWS에서 운영중이었고 GCP에 새로 환경을 구축하게 되면서 **multi-cloud 환경** 경험, **Cloud/k8s 환경에 직접 인프라 구축**, Data Scientist/Analyst 와 협업을 통해 그들의 개발 환경(Jupyter Notebook, pandas 등)을 경험, 서비스 측면에서 다양한 사용자들(임원, 데이터 분석가, 영업 및 마케팅 실무자)의 요구에 맞는 기획 및 구현 방법을 고민하고 개발, 지도 시각화 및 지리 정보 관련 데이터 처리 및 개발
{% if show_portfolio %}
- 포트폴리오: [YoDa](./portfolio/yoda)
{% endif %}