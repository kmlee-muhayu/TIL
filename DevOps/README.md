# CI/CD
* 개발자가 코드를 수정하고 빌드와 테스트, 배포까지 한다면 상당히 많은 시간이 소요될 것이다.
* 코드를 push하는 것만으로 누군가가 빌드, 테스트, 배포까지 자동으로 해준다면 시간을 단축시키고 개발에 더 많은 시간을 들일 수 있을 것이다.
### CI (Continuous Integration; 지속적 통합)
* 빌드/테스트 자동화 과정
* 지속적 통합의 실행
    * 소스/버전 관리 시스템에 대한 변경 사항을 정기적으로 커밋하여 모든 사람에게 동일 작업 기반을 제공하는 것으로 시작
    * 커밋할 때마다 **빌드와 일련의 자동 테스트**가 이루어져 동작을 확인하고 변경으로 인해 문제가 생기는 부분이 없도록 보장
    * CI/CD 파이프라인을 구현하기 위한 첫 번째 단계
### CD (Continuous Delivery; 지속적 서비스 제공, Continuous Deployment; 지속적인 배포)
* 배포의 자동화 과정
* 때로 얼마나 많은 자동화가 이루어지고 있는지 설명을 위해 별도로 사용하기도 함
* 코드 변경이 파이프라인의 이전 단계를 모두 성공적으로 통과하면 **수동 개입 없이 해당 변경 사항이 프로덕션에 자동으로 배포됨**
* 간단한 코드 변경이 **정기적으로 마스터에 커밋**되고, 자동화된 빌드 및 테스트 프로세스를 거치며 다양한 사전 프로덕션 환경으로 승격되며, **문제가 발견되지 않으면 최종적으로 배포됨**
### CI/CD 종류
* **Jenkins**
* **CircleCI**
* **TravisCI**
* **Github Actions**
