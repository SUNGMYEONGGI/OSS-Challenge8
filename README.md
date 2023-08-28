### Challenge8. Github Actions로 DevOps 구축

<h2>💁🏻‍♂️ 목표</h2>

#### 도전과제는 DevOps입니다.
DevOps는 개발과 운영을 통합하고 자동화하는 관행입니다. 어떻게 Github의 코드가 여러 단계를 거쳐 최종 배포 과정까지 자동화되는지 DevOps 전체 흐름을 이해하고 구현합니다
<h2>📚 TO-DO</h2>

- [x] DevOps 이해, 왜 필요한지 설명
      
- [x] `도전과제 7`까지 작성한 Flask 웹앱 리포지토리 Github Actions에서 workflows 구성
  - [x] `workflow 코드힌트1` 참조
        
- [x] Code가 push 또는 PR 되면 workflow 실행을 확인
      
- [x] Branch 보호 규칙 설정
  - [x] 리포지토리에 branch protection rule 설정
  - [x] main branch에 Require a pull request before merging 설정
  - [x] Require approvals - 1명 설정
  - [x] Require status checks to pass before merging 설정
  - [x] Require branches to be up to date before merging 설정
     
- [x] issue를 생성하고 branch 작업
  - [x] template으로 issue를 생성
  - [x] 출력 문자열 “hello”를 “hi”로 변경하는(아무거나) issue 생성
  - [x] issue 처리를 위한 branch 생성
  - [x] branch를 fetch 후 src/test 코드 작업 후 push
     
- [x] PR을 생성 하고 Merge
  - [x] PR을 template으로 생성
  - [x] Github Workflow 자동 수행/검증 확인
  - [x] Code review를 위해 Setting - collaborator로 조원을 1명 추가(수락 필요)
  - [x] 조원의 review 후 approval 되면 merge 수행
  - [x] Merge 후 branch 삭제
  - [x] Issue 자동 close 확인

- [ ] 로컬 개발 머신에서 Docker 이미지를 만들고 테스트
  - [ ] Github에서 issue를 생성 / branch  생성 / fetch 후 branch에서 작업
  - [ ] 자신의 개발 머신에 docker 환경 구성 (WSL 권장)
  - [ ] Dockerfile을 이용해 docker 구성(힌트 참조)
  - [ ] 로컬 개발 머신에서 Docker를 실행하고 테스트
      
- [ ] 클라우드 서비스 credential을 Github에 리포지토리 secret에 추가
  - [ ] CSP의 절차대로 credential을 생성하고 secret에 추가
        
- [x] 빌드 배포 workflow 처리
  - [x] workflow 파일 생성(Workflow 코드 힌트2 참조)
  - [x] workflow의 secret variable을 Github에 추가해 둔 secret으로 설정
  - [x] 코드를 commit 하고 branch로 push
  - [x] Github에서 PR을 템플릿으로 생성하면 자동으로 Action 실행
  - [ ] 배포가 완료되면 CSP의 URL에서 결과를 테스트
  - [ ] 동료 1인의 리뷰 후 merge 수행
        
- [ ] 자동 배포가 아닌 수동 배포 설정
  - [ ] Build - Docker registry 까지만 수행하고 Deploy는 사람의 확인 후 배포하도록 변경

<h2>💡 힌트</h2>

**1️⃣ [Github workflow template - Building and testing Python](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python)**

**2️⃣ Azure CLI([How to install the Azure CLI | Microsoft Learn](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli))**

**3️⃣ Azure 인증 대안: Service Principal**

**4️⃣ Azure Container Registry(https://azure.microsoft.com/ko-kr/products/container-registry)**

**5️⃣ Azure ACI([Azure의 서버리스 컨테이너 - Azure Container Instances | Microsoft Learn](https://learn.microsoft.com/ko-kr/azure/container-instances/container-instances-overview))**

**6️⃣ python flask 앱을 ACI로 배포([A Simple Guide to Deploying a Dockerized Python app to Azure | Towards Data Science](https://towardsdatascience.com/a-simple-guide-to-deploying-a-dockerized-python-app-to-azure-29753ee507eb))**

**7️⃣ Flask app 또는 FastAPI([파이썬 서버 포트(127.0.0.1) 띄우는 방법 비교 정리(FastAPI, Flask)](https://jimmy-ai2.tistory.com/7))**

**8️⃣ NHN클라우드 - Github Actions 배포([Github Actions으로 배포 자동화하기](https://meetup.nhncloud.com/posts/286))**
