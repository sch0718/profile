{% assign image_path = '/assets/images/metrom' | relative_url %}

# Metrom (Hybrid-Cloud 개발 환경 자동화 구축 서비스)

## Metrom?

“CI/CD pipeline과 MSA를 고려한 Self-serving PaaS 제품으로써, Hybrid-Cloud를 지향하는 개발환경 구축 솔루션”

- Phoenix server pattern을 위한 개발환경 구축 솔루션

## 기대효과

### 정량 효과

**개발 1인당**

- 개발환경 구축 연간 10회
- 1회당 평균 3일 소요 (1~10일)
- 연간 30일 근무 손실 (근무일의 12.5%)
- 중급 개발자 기준 연간 750만원 인건비 낭비

### 정성 효과

- 개발환경 불일치로 인한 장애 오류 예방
    - 예) Dev에서는 정상이지만, Test에서는 에러 발생
- 개발자 개인 역량에 의한 환경 셋업 한계 극복
    - 예) 인프라 지식이 없는 개발자의 셋업도 상향 평준화
- 전사적인 개발환경 일관성 확보
    - 예) 전사적인 최적화 정책의 다양한 시도 및 적용 가능

> **개발자 20인 보유 기업의 경우, 연간 1.5억 효과** => **개발자 업무 만족도, 업무 집중도 상승**

## 개발환경 구축에 따른 불만 또는 비효율 발생 원인

![개발환경 구축에 따른 불만 또는 비효율 발생 원인]({{ image_path }}/metrom1.png)

## 주요기능

1. Self-service-Platform As A Service
    - 배포가 가능한 수준으로 잘 만들어진 인프라 구성을 인프라 엔지니어의 도움 없이도 직접 생성하여 개발을 진행 할 수 있도록 도와주는 Self-PaaS(Self-service Platform As A Service)시스템
2. Hypervisor Auto-Provisioning for Private Cloud
    - 내부 네트워크 환경의 Linux 자원을 가상화가 가능한 Hypervisor로 자동 구축. Web UI를 통해 Private Cloud 형태로 관리
3. Lock-in Free everywhere
    - 표준화 되어있는 Docker & Docker-compose를 템플릿화 하여, 특정 Infra 환경에 의존적이지 않도록 구성
        - *Cloud Lock-in free: 특정 Cloud service에 Lock-in 되지 않도록 구성을 표준화 하였으며, 서비스 경쟁력을 기반으로 사용자가 편리하게 선택 가능
4. Build-Test-Run
    - 템플릿화 되어있는 인프라 구성은 개발/테스트/운영의 용도로 사용 가능  
        - *CI/CD pipeline을 위한 DevOps Tool-chain 사용가능. CI/CD pipeline의 시각화를 위한 UI 개발 진행중: Project Loops
5. Cloud Brokerage System
    - 각 Public Cloud service의 연결을 중앙화하여 관리가능. Multi cloud resource monitoring
        - *현재 AWS만 지원. GCP, Azure, Softlayer, Alibaba cloud Plugin은 향후 추가 개발예정
6. Cloud base-camp
    - IDC등 내부 시스템 환경을 Backup system 용도로 구축하여, 각 Public Cloud에 Service를 Up & Off 하는 기반 구축
7. Efficient resource management(TBD)
    - 유휴자원에 대한 관리 및 스케쥴링을 통해 과금을 최소화 하는 방향으로 서비스 제공
        - 예) 생성된 자원은 Aging이 적용되어 생성 후 일정기간이 지나면 자동삭제 됨. 사용자가 주로 업무하는 시간에만 개발 환경이 켜지고, 업무시간이 지나면 꺼짐

## Solution 개발 배경

1. DevOps 문화의 확산 및 프로세스의 연구
    - DevOps 전문가로 구성된 조직의 입장에서, DevOps tool-chain의 활용 및 CI/CD pipeline 구축 노하우를 시스템으로 구현
2. CI/CD
    - CI/CD pipeline에서 중요하게 다루는 배포 단위를 Docker container로 정의하고, Dev/Staging/Production 단계별로 Delivery 할 수 있는 Immutable(불변하는) Infra를 생성하는 목표가 생김
3. Phoenix server pattern
    - 완성된 Immutable infra를 개선하는 방향의 Life-Cycle로써 Phoenix server pattern의 적용이 필요
4. MSA
    - 대단위의 Legacy system을 개발/개선하기 위한 Source code의 관리 또는 Build system을 유지하려 하기 보다는, MSA(Micro Service Architecture)형태로 새로운 서비스를 추가 개발하여 Legacy에 붙여 나가는 방식으로 설계 가이드
5. Managed Cloud service
    - 구축 및 사용이 쉬운 Public Cloud Service라고 할지라도 담당자가 필요하고 전문가가 필요한 현실적 문제점을 최소화 하고자 함
6. 작은 조직구성, 짧은 개발 주기, 빈번한 배포
    - Functional team의 제한적인 인적 구성을 극복하고, 빈번한 배포를 지원하기 위한 공통의 인프라 관리도구의 필요

## 주요 활용방안

1. Market place(TBD)
    - Market-place(향후 개발 예정. 현재 공통 템플릿으로 제공)에 사용자들이 등록한 템플릿을 복제하여 사용
2. Bakery part (DevOps engineering 역할 필요)
    - 운영중인 서비스의 Infra구성을 Docker & docker compose 형태로 제작하여 배포가 가능한 Immutable infra 제작
3. 자유도 높은 개발자 환경
    - Container 형태로 제공되는 개발환경은 개발자에 의해 추가 구성을 할 수 없는 제약이 존재(컨테이너 내부에 다시 컨테이너를 올릴 수 없기 때문), 따라서 별도의 VM을 통해 네트워크 충돌(IP 및 Port 등)을 회피하며, 추가 구성이 필요한 Feature 를 Docker container 형태로 추가하여 템플릿에 반영
4. 개발자에 의한 Immutable infra 생성/관리
    - SCM에 별도의 docker-compose.yml 등을 등록하여 DevOps engineer가 제공하는 템플릿이 아닌, 개발자가 직접 구성한 인프라 구성을 생성
5. Baremetal to Multi-Cloud to Back
    - 내부 유휴 자원 등을 활용하여 개발이 완료된 Immutable infra를 Public cloud로 배포하고, Public cloud상에서 발생하는 Data Update를 다시 내부 자원으로 Replication & Backup 하는 형태로 원천 Data를 내부에 유지 관리. 다수의 Cloud service중 상황에 따라 선택적으로 Service를 Migration 할 수 있도록 모듈화
6. Auto Provisioning
    - VM 생성 시, 시스템에 필요한 기본 어플리케이션의 설치 및 템플릿에 명시된 인프라 구성과, 개발에 필요한 Source code를 SCM(git, svn 등)으로부터 Clone 하여 바로 개발
7. QA 환경
    - 개발이 완료된 Immutable infra를 검증하기 위한 QA 환경으로 활용

## 기타 활용방안

1. 교육 실습 환경 구축
    - 순간적으로 필요한 실습용 자원을 생성 후 정리하는 패턴으로 내부자원 효율적 활용
2. 내부 인프라 자원 강화
    - 기존 보유중인 대량의 컴퓨팅 자원을 PaaS 형태로 활용(예. 자체 호스팅 시스템)
3. 망분리 환경에서의 외부 개발 플랫폼 구축
    - 높은 수준의 보안권고(금감원 기준)를 준수하기 위한 망분리 환경의 CI/CD Pipeline 구축 1차 단계 적용
4. 개인 홈네트워크 구축
    - NAS/Plex 등 개인의 홈네트워크 구축을 위한 템플릿 활용
5. Web IDE를 통한 개발
    - Start from scratch 형태로 별도의 Infra 구성 없이 개발을 시작하는 사용자를 위한 웹서비스 상의 개발 환경제공
6. 사설 게임서버
    - 중/소단위 게이머 그룹을 위한 사설 게임서버 활용

## What is the Metrom?

![What is the Metrom?]({{ image_path }}/metrom2.png)

## Metrom Service Architecture Overview

[![Architecture Overview]({{ image_path }}/metrom3.png)](https://www.youtube.com/watch?v=544y4QNa70g){:target="_blank"}

[원본 영상](https://www.youtube.com/watch?v=544y4QNa70g)

## Metrom Service 화면

### Dashboard

![Dashboard]({{ image_path }}/metrom4.png)

### Resource management

![Resource management]({{ image_path }}/metrom5.png)

### VM Create

![VM Create]({{ image_path }}/metrom6.png)

### PaaS management

![PaaS management]({{ image_path }}/metrom7.png)

### 서비스 시연 영상

- APM: [원본 영상](https://www.youtube.com/watch?v=NlNKjP0gbbs)  
  [![APM](https://img.youtube.com/vi/NlNKjP0gbbs/0.jpg)](https://www.youtube.com/watch?v=NlNKjP0gbbs){:target="_blank"}
- Eclipse Che: [원본 영상](https://www.youtube.com/watch?v=lRIVLFltws0)  
  [![Eclipse Che](https://img.youtube.com/vi/lRIVLFltws0/0.jpg)](https://www.youtube.com/watch?v=lRIVLFltws0){:target="_blank"}
- NextCloud: [원본 영상](https://www.youtube.com/watch?v=9bYkeaDSdFs)  
  [![NextCloud](https://img.youtube.com/vi/9bYkeaDSdFs/0.jpg)](https://www.youtube.com/watch?v=9bYkeaDSdFs){:target="_blank"}