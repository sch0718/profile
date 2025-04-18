{% assign image_path = '/assets/images/mc_gaudi' | relative_url %}

# MC Gaudi (DevOps 서비스)

## 2019 Pivotal Cloud Native Day 발표 영상

[![발표 영상](https://img.youtube.com/vi/F_GFwZRAaM8/0.jpg)](https://youtu.be/F_GFwZRAaM8?si=AxXgPWSd_k1J8khn){:target="_blank"}

[원본 영상](https://youtu.be/F_GFwZRAaM8?si=AxXgPWSd_k1J8khn)

## 제품 소개

McGaudi는 업무 프로세스와 도구 등을 DevOps 관점에서
최적의 조건으로 구성하여 자동화 처리하고, 개발 업무 결재 관리에
대한 부분을 통합적으로 다룸으로써 빠른 개발/빠른 출시를 위한
최적의 솔루션입니다.

DevOps는 하나의 큰 문화이면서, 개발 관련 업무 프로세스, 방법론, 도구 등에 관련한 전체의 틀 역할로써 시장의 빠른 변화를 따라가기
위한 최선의 전략입니다. 따라서 DevOps는 모범사례(Best Practice)를 기반으로 다양한 시도를 통한 최적의 업무 프로세스를
구축하고, 관련한 도구를 구성하여 자동화된 시스템을 기반으로 개발 문화를 새롭게 하는 것에 필수적인 요소입니다.

### 엔터프라이즈 서비스 애플리케이션의 개발 및 검증/배포를 사용자 관점에서 쉽게

체계화된 업무 프로세스를 CI/CD pipeline과 연동하여, 개발 요청부터 배포까지 전체 업무를 하나의 과정으로 관리
Well-made CI/CD pipeline template을 통해 간단한 정보 입력만으로도 프로젝트별 업무 프로세스를 쉽게 생성 및 관리
잘 정리된 업무 프로세스를 기반으로 DevOps 문화와 기술 습득에 도움을 줍니다.

### McGaudi와 함께라면?

- 빠르고 간소화된 결재 프로세스 및 시스템 제공
- CI/CD를 위한 단일화된 화면 제공
- 다양한 관점(개발 요청/개발/빌드/검증/배포)의 자동화된 흐름의 시각화
- 모바일 서비스 환경을 기반으로 편리한 Remote office & work가 가능
- QA 자동화를 위한 기반 프로세스 제공
- DevOps 문화 도입을 위한 손쉬운 접근

> **개발 요청에서 처리까지 소요되는 시간**
> 
> ![Development Cycle Change]({{ image_path }}/product_desc_dev_cycle.png)

### McGaudi Life Cycle

비즈니스의 요구 사항을 단일화된 채널을 통해 처리할 수 있으므로, 개발 업무 진행에 따른 시스템 구성 등을 시각적으로 확인할 수 있습니다. 또한, 자동화 처리된 빌드/검수 환경 제공 등을 통해 신속한 검수 및 서비스 반영이 가능하도록 모든 과정을 한곳에서 관리합니다.

![McGaudi Life Cycle]({{ image_path }}/product_desc_mc_gaudi_life_cycle.png)

### Architecture Overview

![Architecture Overview]({{ image_path }}/install_arch.png)

### McWrapper?

McWrapper는 사용자에게 개발 업무 결재 프로 세스를 확인 및 요청/처리 등을 하는 창구 역할을 합니다. 이 해당 창구를 통해 McGaiver의 CI/CD Pipeline를 기반으로 개발/배포 시스템을 자동으로 처리합니다.

- McWrapper를 통한 요청에서 배포까지의 그룹 및 관계  
    [![Group & Releationship for request to release via the McWrapper](https://img.youtube.com/vi/Wgw8eMYbj5c/0.jpg)](https://youtu.be/Wgw8eMYbj5c){:target="_blank"}  
    [원본 영상](https://youtu.be/Wgw8eMYbj5c)
- Workflow  
    ![WorkFlow]({{ image_path }}/workflow.png)
    - Workflow 흐름에 따른 git 브랜치 동작 방식  
        [![How to work on the git branch by McWrapper](https://img.youtube.com/vi/5lVDMMUdZmw/0.jpg)](https://youtu.be/5lVDMMUdZmw){:target="_blank"}  
        [원본영상](https://youtu.be/5lVDMMUdZmw)
- MSA(MicroService Architecture) Version  
    ![MSA Architecture]({{ image_path }}/msa_architecture.png)
- Monolithic Version  
    ![Monolithic Architecture]({{ image_path }}/monolithic_architecture.png)

---

## 사용자 매뉴얼

### 용어 설명

#### 사용자

| 한국어 | English |
| ------ | ------- |
| 사용자 | User    |

McWrapper에 가입되어 사용하는 사람입니다.

#### 로그인

| 한국어 | English |
| ------ | ------- |
| 로그인 | Sign In |

[사용자](#사용자) 계정 인증을 통해 사이트 이용을 시작합니다.

#### 로그아웃

| 한국어   | English  |
| -------- | -------- |
| 로그아웃 | Sign Out |

[사용자](#사용자) 계정 정보를 통한 사이트 이용을 종료합니다.

#### 그룹

| 한국어 | English |
| ------ | ------- |
| 그룹   | Group   |

[사용자](#사용자)들이 소속된 집단으로써, 특정 [사용자](#사용자)들을 일괄적으로 지정하기 위한 단위입니다.

#### 워크스페이스

| 한국어       | English   |
| ------------ | --------- |
| 워크스페이스 | Workspace |

[프로퍼티](#프로퍼티)와 [프로젝트](#프로젝트)가 생성되는 공간으로써, 생성된 모든 콘텐츠는 워크스페이스 단위로 공유됩니다.

#### 프로퍼티

| 한국어   | English  |
| -------- | -------- |
| 프로퍼티 | Property |

비즈니스적으로 구분되는 상품이나 자산의 최상의 단위로써, [스토리북](#스토리북)을 통해 업무 요건을 생성 및 관리할 수 있습니다. (ex. 검색, 지도, 카페, 블로그, etc.)

#### 프로젝트

| 한국어   | English |
| -------- | ------- |
| 프로젝트 | Project |

개별적인 산출물을 생성하는 소프트웨어 개발의 단위이며, [릴리즈 티켓](#릴리즈-티켓)을 통해 개발 활동과 개발 주기를 관리할 수 있습니다.

#### 구성원

| 한국어 | English |
| ------ | ------- |
| 구성원 | Member  |

[그룹](#그룹) 또는 [워크스페이스](#워크스페이스) 등에 소속된 구성원입니다.

#### 빌드

| 한국어 | English |
| ------ | ------- |
| 빌드   | Build   |

소스 코드로부터 실행 가능한 소프트웨어로 만듭니다.

#### 산출물

| 한국어 | English  |
| ------ | -------- |
| 산출물 | Artifact |

[빌드](#빌드) 된 결과물입니다.

#### 요청자

| 한국어 | English   |
| ------ | --------- |
| 요청자 | Requester |

비즈니스 담당자(현업) 또는 Product Owner 등 개발이 필요한 사항들을 요청하는 사람입니다.

#### PL

| 한국어 | English |
| ------ | ------- |
| PL     | PL      |

Project Leader. [프로젝트](#프로젝트) 내 개발을 Leading 하고, 설계하는 사람입니다.

#### 검수 담당자

| 한국어      | English |
| ----------- | ------- |
| 검수 담당자 | QA      |

Quality Assurance. 개발된 [산출물](#산출물)의 품질 및 테스트를 관리하고 승인하는 역할입니다.

#### 배포 담당자

| 한국어      | English  |
| ----------- | -------- |
| 배포 담당자 | Deployer |

검증된 소프트웨어를 실제 운영환경에 [배포](#배포)할지 결정하는 사람입니다.

#### 릴리즈

| 한국어 | English |
| ------ | ------- |
| 릴리즈 | Release |

[프로젝트](#프로젝트)를 통해 개발된 소프트웨어 또는 서비스를 공개하는 단위입니다.

#### 배포

| 한국어 | English |
| ------ | ------- |
| 배포   | Deploy  |

검증된 [산출물](#산출물)을 실제 운영환경에 반영합니다.

#### 롤백

| 한국어 | English  |
| ------ | -------- |
| 롤백   | Rollback |

[배포](#배포)한 [산출물](#산출물)에 대하여 문제가 발생했을 경우 이전 버전으로 되돌리는 작업입니다.

#### 업무

| 한국어 | English |
| ------ | ------- |
| 업무   | Task    |

전체 업무를 포괄하는 최상위 단위입니다.

#### 티켓

| 한국어 | English |
| ------ | ------- |
| 티켓   | Ticket  |

업무 처리를 위해 요청사항을 담당자에게 전달하고 일련의 처리 과정을 기재하여 처리 과정과 결과를 조회할 수 있도록 정리한 게시물입니다.

#### 스토리북

| 한국어   | English   |
| -------- | --------- |
| 스토리북 | StoryBook |

[요청자](#요청자)가 [프로퍼티](#프로퍼티)의 요건에 대한 [유저 스토리](#유저 스토리)를 모아 놓은 업무 단위입니다. (현업의 요건을 모아놓은 업무 단위입니다.)

#### 유저 스토리

| 한국어      | English    |
| ----------- | ---------- |
| 유저 스토리 | User Story |

현업의 구체적인 요건 사항이며, [프로퍼티](#프로퍼티)에서 수행해야 하는 기능을 프로퍼티 사용자의 관점에서 상세히 기술한 요구 사항입니다.

#### 릴리즈 티켓

| 한국어      | English        |
| ----------- | -------------- |
| 릴리즈 티켓 | Release Ticket |

[릴리즈](#릴리즈) 과정(process) 및 상태를 보여주고, CI/CD 시스템과 연동하는 [티켓](#티켓)입니다.

#### 개발 티켓

| 한국어    | English    |
| --------- | ---------- |
| 개발 티켓 | Dev Ticket |

개발 과정(process) 및 상태를 보여주고, 관리하는 [티켓](#티켓)입니다.

#### 업무 담당자

| 한국어      | English  |
| ----------- | -------- |
| 업무 담당자 | Assignee |

[스토리북](#스토리북) 또는 [티켓](#티켓)의 진행을 맡아 현재 업무 처리를 수행하고 있는 사용자입니다.

#### 참조자

| 한국어 | English |
| ------ | ------- |
| 참조자 | Cc      |

[스토리북](#스토리북) 또는 [티켓](#티켓)의 작성자나 담당자는 아니지만, 진행 상황을 관찰하는 사람입니다.

#### 파이프라인

| 한국어     | English  |
| ---------- | -------- |
| 파이프라인 | Pipeline |

CI와 CD가 수행되는 절차를 정의하고 정의된 절차에 맞춰 자동으로 반응하여 개발 생애 주기를 관리하는 단위입니다.

#### CI

| 한국어 | English |
| ------ | ------- |
| CI     | CI      |

개발자를 위한 자동화 프로세스인 지속적인 통합(Continuous Integration)을 의미합니다. CI를 성공적으로 구현할 경우 애플리케이션에 대한 새로운 코드 변경 사항이 정기적으로 [빌드](#빌드) 및 테스트 되어 공유 저장소에 병합되므로 여러 명의 개발자가 동시에 애플리케이션 개발과 관련된 코드 작업을 할 경우 서로 충돌할 수 있는 문제를 해결할 수 있습니다.

#### CD

| 한국어 | English |
| ------ | ------- |
| CD     | CD      |

지속적인 서비스 제공(Continuous Delivery) 또는 지속적인 배포(Continuous Deployment)를 의미하며 이 두 용어는 상호 교환적으로 사용됩니다. 두 가지 의미 모두 [파이프라인](#파이프라인)의 추가 단계에 대한 자동화를 뜻하지만 때로는 얼마나 많은 자동화가 이루어지고 있는지를 설명하기 위해 별도로 사용되기도 합니다.

#### 파이프라인 변수

| 한국어          | English           |
| --------------- | ----------------- |
| 파이프라인 변수 | Pipeline Variable |

패스워드, 인증서 관련 정보 등을 포함한 보안이 필요한 정보입니다.

# 메뉴 설명

![Menu]({{ image_path }}/menu_desc.png)

![GNB - 01]({{ image_path }}/menu_desc_gnb01.png)

![GNB - 02]({{ image_path }}/menu_desc_gnb02.png)

- 관리자(Administrator)
  - 그룹 관리(Manage groups): [그룹](#그룹)을 관리하고, [구성원](#구성원)을 추가하거나 제외합니다.
  - 권한 관리(manage permissions): 권한에 [그룹](#그룹)을 할당하거나 조회합니다.
  - 사용자 관리(Manage users): [사용자](#사용자)를 관리하고, 조회합니다.
  - 초대자 관리(Manage guests): 초대 메일을 전송/재전송하고, 초대 정보를 관리합니다.
- 사용자(User)
  - 워크스페이스(Workspace): [워크스페이스](#워크스페이스) 목록이 출력됩니다. 관리자 권한이 있으면, 우측에 Management 메뉴가 보입니다.
  - 프로퍼티(Property): [프로퍼티](#프로퍼티) 목록이 출력됩니다. 관리자 권한이 있으면, 우측에 Management 메뉴가 보입니다.
  - 프로젝트(Project): [프로젝트](#프로젝트) 목록이 출력됩니다. 관리자 권한이 있으면, 우측에 Management 메뉴가 보입니다.
- 데브옵스(DevOps)
  - 기본 파이프라인 변수 설정(Default pipeline variable settings): 자주 사용되는 [파이프라인 변수](#파이프라인-변수)를 관리합니다.
  - 파이프라인 관리(Manage pipelines): [파이프라인](#파이프라인)을 관리합니다.
- Support
  - 사용자 도움말(User Guide): McWrapper의 사용자 매뉴얼
- 상단 메뉴(GNB)
  - Home: 사이트의 메인 페이지로 이동합니다.
  - 알림(Notifications): 나에게 도착한 알림 메시지를 조회하고, 클릭하여 관리 화면으로 이동하는 인터페이스를 제공합니다.
  - Create ...: 생성 권한이 있는 [워크스페이스](#워크스페이스), [프로퍼티](#프로퍼티), [프로젝트](#프로젝트), [스토리북](#스토리북), [릴리즈 티켓](#릴리즈-티켓)을 생성합니다.
  - Profile: [사용자](#사용자) 정보를 조회하고, 수정합니다.

### 역할 별 사용방법

#### 일반 사용자

##### 회원 가입

회원 가입은 초대된 이메일 주소로 발송된 링크를 통해서만 할 수 있습니다.

![회원 가입]({{ image_path }}/join.gif)

링크를 클릭하여 페이지 이동 후 원하는 가입 방법을 선택해 사용자 정보를 입력하시면 됩니다.

##### 로그인

McWrapper는 다양한 방식의 로그인을 지원 할 예정입니다.(현재 Google OAuth 2.0을 지원합니다.)

- OAuth 2.0(Google, Github, Facebook, Naver, Kakao 등)
- ID / PW Form 로그인
- LDAP
- ETC...

##### 인터페이스

![인터페이스 - 01]({{ image_path }}/interface_01.png)

1. 메인 페이지로 이동합니다.
2. 나에게 온 알림의 개수를 보여줍니다.
3. 권한이 있는 [스토리북](#스토리북), [릴리즈 티켓](#릴리즈-티켓) 등을 생성합니다.
4. 전체 메뉴를 펼칩니다.

![인터페이스 - 02]({{ image_path }}/interface_02.png)

5. 사용자 조회 페이지로 이동합니다.
6. 언어를 변경합니다.
7. 사이트 이용을 종료합니다.
8. 펼쳐진 메뉴를 닫습니다.

![인터페이스 - 03]({{ image_path }}/interface_03.png)

9. 이전 페이지로 이동합니다.
10. 메인 페이지로 이동합니다.
11. 페이지의 타이틀이 표시됩니다.
12. 페이지를 리로드 합니다.
13. 옵션 기능이 있는 경우 표시됩니다.

#### 사이트 관리자(Administrators)

사이트 관리자 권한은 시스템이 설치된 후 첫 번째 로그인한 사용자에게 부여됩니다.

![사이트 관리자]({{ image_path }}/administrator_01.gif)

##### 사용자 초대

초대 관리 메뉴에서 이메일 주소를 이용하여 사용자를 초대할 수 있습니다.

![사용자 초대]({{ image_path }}/invite_users_01.gif)

여러 사람을 동시에 초대할 수 있고, 초대와 동시에 가입 시 소속될 그룹이나 워크스페이스를 미리 지정할 수도 있습니다.

![사용자 그룹 초대]({{ image_path }}/invite_users_02.gif)

이미 초대된 사용자에게 초대 메일을 재발송 하거나 초대 정보를 삭제할 수 있습니다.

![초대 메일 재발송]({{ image_path }}/invite_users_03.gif)

초대 정보가 삭제된 사용자는 메일의 링크를 통해 가입을 시도하더라도 가입이 불가합니다.

##### 그룹 관리 & 권한 관리

시스템에 미리 정의된 그룹들이 존재합니다. 이 그룹들은 삭제가 불가합니다.

- Administrators: 사이트의 관리자 그룹입니다.
- DevOps: DevOps 메뉴에 접근 권한을 가지는 그룹입니다.
- WorkspaceManagers: [워크스페이스](#워크스페이스) 생성 권한을 가지는 그룹입니다.
- Users: 가입된 후 사용자들이 속하게 되는 기본 그룹. 다른 그룹에 소속되면 제외됩니다.

시스템에서 관리되는 그룹들과 별도로 커스텀 그룹을 만들고, 사용자를 추가할 수 있습니다.

![커스텀 그룹 생성]({{ image_path }}/create_group.gif)

커스텀 그룹을 통해 쉽고, 빠르게 사용자들의 권한을 관리할 수 있습니다.

##### 권한 관리

미리 정의되어 있는 권한에 그룹을 연결하여 사용자에게 권한을 부여합니다.

예를 들어, DevOps 엔지니어가 아닌 PL의 경우 DevOps 엔지니어들이 만들어 놓은 파이프라인을 조회하여 참고할 필요가 있는데 이때 PL 그룹을 만들고, 해당 사용자들을 추가한 후 DevOps > Pipeline view 권한을 PL 그룹에 부여하면 PL 그룹에 소속된 구성원들은 파이프라인의 조회가 가능해집니다.

![커스텀 그룹 활용]({{ image_path }}/group_permission.gif)

#### 데브옵스 엔지니어(DevOps Engineers)

데브옵스 엔지니어는 CI/CD [파이프라인](#파이프라인) 템플릿을 작성하고, 관리하는 역할을 합니다.

Manage pipelines 메뉴에서 파이프라인 템플릿을 작성하고, 약속된 규약에 따라 작성된 [파이프라인 변수](#파이프라인-변수)들을 프로젝트별로 다르게 입력하여 프로젝트마다 파이프라인을 작성해야 하는 수고를 덜 수 있습니다.

##### Default pipeline variable settings

Default pipeline variable settings 메뉴에서는 자주 사용되고, 개인 정보가 아닌(ex. 이메일 주소, 패스워드 등) [파이프라인 변수](#파이프라인-변수)들의 값을 미리 설정해 놓을 수 있습니다.

예를 들어, [빌드](#빌드) 된 [산출물](#산출물)을 팀 또는 사내에서 운영하는 Docker Registry에 Push 하는 프로세스가 파이프라인에 자주 사용된다면 Docker Registry 주소나 계정 정보를 반복적으로 입력해야 합니다.

이때, Default pipeline variable settings 메뉴에 [파이프라인 변수](#파이프라인-변수)로 등록해 놓으면 [파이프라인 변수](#파이프라인-변수) 등록 시 자동으로 입력되기 때문에 [프로젝트](#프로젝트)마다 일일이 등록하지 않아도 됩니다.

또, 1Depth YAML 형태로 한 번에 [파이프라인 변수](#파이프라인-변수)를 등록하는 편의 기능도 제공이 됩니다.

```yml
docker_registry_adderess: registry.mycorporation.com # Docker Registry Address
profile_active_dev: dev # development env active profile
profile_active_stg: stg # staging env active profile
profile_active_prd: prd # production env active profile
```

![기본 파이프라인 변수 등록 - 01]({{ image_path }}/default_pipeline_variable_01.gif)

[파이프라인 변수](#파이프라인-변수)를 등록한 후 패스워드와 같이 노출되면 안 되는 값들은 마스킹 처리를 하여 줍니다.

실제 데이터에는 마스킹 여부와 상관없이 모두 암호화됩니다.

![기본 파이프라인 변수 등록 - 02]({{ image_path }}/default_pipeline_variable_02.gif)

##### Manage pipelines

다양한 형태의 [파이프라인](#파이프라인)을 템플릿화 하여 등록하고, [프로젝트](#프로젝트)에서 고유의 값을 가지는 변수들을 입력할 수 있도록 [파이프라인 변수](#파이프라인-변수)들을 설정합니다.

![파이프라인 템플릿 관리 - 01]({{ image_path }}/manage_pipeline_01.png)

파이프라인의 성격에 맞는 태그를 달아놓으면 검색에 용이합니다.

자세한 파이프라인 작성 방법은 [파이프라인 작성 방법](#파이프라인-작성-방법)을 참조하시기 바랍니다.

![파이프라인 템플릿 관리 - 02]({{ image_path }}/manage_pipeline_02.png)

파이프라인에 등록된 [변수](#파이프라인-변수)들의 값과 마스킹 여부, [프로젝트](#프로젝트)에서 수정 가능 여부를 설정합니다.

수정 불가로 설정할 경우 프로젝트 파이프라인 설정 화면에서는 해당 변수는 출력되지 않습니다. 그렇기 때문에 수정 불가로 설정할 경우 반드시 값이 있어야 합니다.

개발된 소스코드가 있는 GIT 저장소의 주소처럼 프로젝트별로 다르게 설정되어야 할 변수들은 수정 가능으로 설정하면 됩니다.

![파이프라인 템플릿 관리 - 03]({{ image_path }}/manage_pipeline_03.gif)

새로 만들려고 하는 파이프라인과 비슷한 파이프라인이 이미 존재할 경우 복사 기능을 활용할 수 있습니다.

복사한 후 변경되어야 할 내용만 수정하면 됩니다.

#### 워크스페이스 관리자(Workspace Managers)

워크스페이스 관리자는 사이트 관리자로부터 [워크스페이스](#워크스페이스) 생성 권한을 부여받습니다. ([사이트 관리자 참조](#그룹-관리-&-권한관리))

![워크스페이스 생성]({{ image_path }}/workspace_manager_01.gif)

워크스페이스를 생성 후 구성원을 추가하여 줍니다.

![워크스페이스 구성원 관리]({{ image_path }}/workspace_manager_02.gif)

각 권한 그룹에 해당 사용자들을 추가하여 줍니다.

![워크스페이스 그룹별 구성원 관리]({{ image_path }}/workspace_manager_03.gif)

#### 프로퍼티 관리자(Property Managers)

프로퍼티 관리자는 [워크스페이스 관리자](<#워크스페이스-관리자(Workspace-Managers)>)로부터 권한을 부여받아 [프로퍼티](#프로퍼티)를 생성할 수 있습니다.

![프로퍼티 생성]({{ image_path }}/property_manager_01.gif)

프로퍼티를 생성 후 [데브데스크](#데브데스크DevDesk) 및 [요청자](<#요청자(Requester)>) 권한 그룹에 해당 사용자들을 추가하여 줍니다.

![프로퍼티 그룹별 구성원 관리]({{ image_path }}/property_manager_02.gif)

#### 프로젝트 관리자(Project Managers)

프로젝트 관리자는 [워크스페이스 관리자](<#워크스페이스-관리자(Workspace-Managers)>)로부터 권한을 부여받아 [프로젝트](#프로젝트)를 생성할 수 있습니다.

![프로젝트 생성]({{ image_path }}/project_manager_01.gif)

프로젝트 생성 후 프로젝트에 맞는 [파이프라인](#파이프라인)을 선택하고, [파이프라인 변수](#파이프라인-변수)를 설정해야 합니다.

![파이프라인 선택 및 변수 등록]({{ image_path }}/project_pipeline_setting.gif)

> **파이프라인 변수 입력 예(Vue 파이프라인)**
>
> ![project-pipeline-01]({{ image_path }}/project-pipeline-reg.png)
>
> 1. git_address(Git 주소): ssh://로 시작되는 git 주소를 입력합니다.
> 2. git_email(Git 계정 이메일 주소): Git 계정 이메일 주소를 입력합니다.
> 3. git_name(Git 계정): Git 계정을 입력합니다.
> 4. git_private_key: Git 계정에 등록된 SSH Key를 입력합니다. ([SSH Key 등록 방법 참조](./ssh_key_register.md))
> 5. profile_active_dev, profile_active_prd, profile_active_stg는 각각 배포 환경에 따라 적용될 profile 값을 넣어주면 됩니다. [Vue CLI 가이드 참고](https://cli.vuejs.org/guide/mode-and-env.html#using-env-variables-in-client-side-code)

#### 요청자(Requester)

요청자는 [프로퍼티 관리자](<#프로퍼티-관리자(Property-Managers)>)로부터 권한을 부여받습니다.

요청자는 업무 담당자들의 다양한 개발 요건들을 모아 스토리북을 작성합니다.

![스토리북 생성]({{ image_path }}/requester_01.gif)

스토리북은 상세 요건인 [유저 스토리](#유저-스토리)를 복수로 가집니다.

[유저 스토리](#유저-스토리)는 [데브데스크](#데브데스크DevDesk)가 요건에 해당하는 [프로젝트](#프로젝트)를 분류하고, [PL](<#PL(Project-Leader)>)에 의해 릴리즈 티켓에 1:1로 연결되어 실제로 상세 요건이 개발, [배포](#배포)되는 과정을 지켜볼 수 있습니다.

![개발 진행중인 스토리북]({{ image_path }}/requester_02.png)

#### 데브데스크(DevDesk)

데브데스크는 [요청자](<#요청자(Requester)>)가 만든 스토리북(#스토리북)의 다양한 요건(유저 스토리)들을 해당 [프로젝트](#프로젝트)에 연결하는 역할을 합니다.

그렇기 때문에 각 요건들이 어떤 프로젝트와 연관성이 있는지 잘 파악하고 있는 사람이 맡아야만 합니다.

![Property-create]({{ image_path }}/devdesk-project-mapping.gif)

#### PL(Project Leader)

PL은 [데브데스크](#데브데스크DevDesk)가 스토리북에 자신의 프로젝트를 연결하면 해당 요건이 반영될 [릴리즈](#릴리즈) 계획에 따라 [릴리즈 티켓](#릴리즈-티켓)을 선택하여 연결합니다.

![스토리북-릴리즈 티켓 연결]({{ image_path }}/storybook_mapping_and_release_ticket.gif)

만약 기존에 만들어진 [릴리즈 티켓](#릴리즈-티켓)의 [배포](#배포) 버전에 포함하지 못한다면 새로운 [릴리즈 티켓](#릴리즈-티켓)을 만들어 연결할 수 있습니다.

![릴리즈 티켓 설계 단계]({{ image_path }}/pl_02.png)

또, [릴리즈 티켓](#릴리즈-티켓)이 만들어지면 해당 요건들에 대한 분석 및 설계를 진행합니다.

![릴리즈 티켓 PL 승인 단계]({{ image_path }}/pl_03.png)

동일한 프로젝트 내에서 [릴리즈](#릴리즈)가 2건 이상 동시에 진행될 경우 Staging 환경에는 하나의 산출물(Artifact)만 배포가 되기 때문에 어떤 [릴리즈 티켓](#릴리즈-티켓)을 진행시킬지 PL이 판단하여 승인 절차를 거치게 됩니다.

먼저 Staging 환경에 [배포](#배포)되었던 [릴리즈 티켓](#릴리즈-티켓)은 Dev Testing 단계로 자동으로 변경됩니다.

모든 Process가 정상적으로 처리된 [릴리즈 티켓](#릴리즈-티켓)은 PL이 종료시킬 수 있습니다.

#### 검수 담당자(Quality Assurance)

검수 담당자는 Staging 환경에 [배포](#배포)된 소프트웨어를 검증합니다.

검증이 완료되면 Production 환경에 배포될 준비가 됩니다.

#### 배포 담당자(Deployer)

배포 담당자는 개발된 소프트웨어를 최종적으로 Production 환경에 [배포](#배포)할지 결정하는 역할을 합니다.

[배포](#배포)된 소프트웨어에 문제가 있을 경우 [롤백](#롤백) 여부를 결정하기도 합니다.

### 릴리즈 티켓 Flow

![릴리즈 티켓 흐름도]({{ image_path }}/McWrapper_Release_Ticket_Flow.png)

![릴리즈 티켓 상태 명세서]({{ image_path }}/McWrapper_Release_Ticket_Status_Speccification.png)

### 파이프라인 작성 방법

#### 파이프라인 구성

![파이프라인 구성]({{ image_path }}/write_pipeline00.png)

pipeline.yml 파일은 크게 Resources 부분과 Jobs 부분으로 구성되어 있습니다. 필요에 의해 위의 그림과 같이 credentials.yml 파일에 보안이 필요하거나 파이프라인 변수들을 별도로 저장하여 불러올 수 있습니다.

##### Resources

[Job](#Jobs)에서 사용할 resource를 정의합니다.

주로 특정 데이터를 불러오는 resource와 작업한 [산출물](#산출물)을 [배포](#배포)하는 resource로 구성되어 있습니다.

##### Jobs

![Job]({{ image_path }}/write_pipeline02.png)

분리된 하나의 실행 단위입니다. Aggregate, Task, Put 순으로 실행됩니다

- **Aggregate**
  Task에서 사용할 resource를 불러옵니다.
  - passed: 현재의 Job이 어떤 Job 이후에 실행될지 정의합니다.
  - trigger: 연결된 resource가 완료될 시 자동으로 현재의 Job이 실행됩니다.
- **Task**
  Job에서의 실행 환경과 source들을 가져올 수 있으며, CLI 명령어를 실행시킬 수 있습니다.
- **Put**
  Task 이후에 실행되는 부분으로써 Resources에 정의된 resource에 [산출물](#산출물)을 [배포](#배포)할 수 있습니다.

#### McWrapper와 연동을 위한 변수들

아래 변수들의 값은 McWrapper에서 자동으로 입력됩니다.

- wrapper_group_name: 파이프라인 그룹명(워크스페이스 ID)
- wrapper_project_code: 프로젝트 코드
- wrapper_ticket_number: 티켓 번호
- ticket_version: 티켓 버전
- rollback_version: 롤백 버전
- callback_url_success: 성공 callback url
- callback_url_fail: 실패 callback url


