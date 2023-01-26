# RDS vs EC2
### RDS 란?
* **AWS RDS는 인프라 및 DB 업데이트를 관리해주는 것 뿐만 아니라 까다로운 관계형 DB의 설치, 운영, 관리를 지원하는 서비스**
* MySQL, MariaDB, Aurora, Oracle, SQL Server, PostgreSQL 데이터베이스 엔진을 지원
  * **Aurora** : Amazon 자체 데이터베이스로, 장애 발생에도 더 안전하고 가용영역을 통해 자체 복구 가능하며, 추가적인 퍼포먼스 기능들을 제공 
* DB의 크기는 기본(`m4`), 메모리 최적화(`r3`), 마이크로(`t2`) 3가지 카테고리로 나뉨
  * 최적화 된 I/O을 실현할 수 있도록 각 그룹마다 특성에 맞게 vCPUs, GiBs 메모리, 네트워크 성능 수준 설정
### RDS 사용 vs EC2에 DB 설치
* 비용적 측면에서는 EC2에 사용중인 데이터베이스를 직접 설치하는 것이 저렴함
* RDS를 사용하게 되면 **빠른 환경 구축**과 **DB 관리를 자동**으로 해준다는 이점이 존재
  * DB 도입 및 관리 측면에서 시간과 노력적인 비용을 아낄 수 있음
* PaaS 서비스의 취약점 중 하나는 사용 중이지 않을 때 상관 없이 계속 비용을 지불해야 했음
  * AWS에서의 RDS 업데이트로 인해 더 이상 사용 중이지 않을 때 불필요한 비용을 지불하지 않아도 됨 
### 정리
* 사용 중인 DB에 대해 정확히 파악하지 않으면 제대로 된 비용을 메길 수 없다.
* RDS는 DB의 백엔드에 대한 관리 및 구축을 지원하면서 시스템 관리를 간소화한다.
  * **DB의 관리보다 애플리케이션에 집중할 수 있다.**
* 인프라 운영을 위한 애플리케이션 또는 제대로 설계된 자동화 시스템, DB 전문 관리팀이 있는 경우 꼭 RDS가 필요하지 않을 수 있다.