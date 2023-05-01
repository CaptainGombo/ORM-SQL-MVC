# ORM-SQL-MVC
 ORM, SQL, MVC 4주차 WIL 간단 정리


# ORM(객체 관계 매핑)
>객체 지향 프로그래밍 언어에서 사용하는 객체와 관계형 데이터베이스의 데이터를 서로 호환되도록 매핑해주는 기술. 
영속성을 갖는 데이터를 저장하고 관리하는 방법 중 하나이며, MVC 패턴에서 모델(MODEL)을 기술하는 도구로 사용된다.

# SQL(구조적 쿼리 언어)
>관계형 데이터베이스에서 정보를 저장하고 처리하기 위한 프로그래밍 언어로, DDL, DML, DCL 등의 명령어로 구성된다.

### DDL(Data Definition Language)
>데이터베이스 객체를 생성, 수정, 삭제하는 명령어를 말함.
데이터베이스의 스키마를 정의하거나 수정하는 역할을 하며, 대표적으로 CREATE, ALTER, DROP 등의 명령어가 있음.

### DML(Data Manipulation Language)
>데이터베이스에서 데이터를 조회, 추가, 수정, 삭제하는 명령어를 말함. 
즉,데이터의 CRUD(Create, Read, Update, Delete) 작업을 수행하는 역할을 한다.
대표적인 DML 명령어로는 SELECT, INSERT, UPDATE, DELETE가 있음.

### DCL(Data Control Language)
>데이터베이스의 사용자에 대한 권한을 관리하는 명령어를 말함.
데이터베이스를 사용하는 사용자들에게 어떤 권한을 부여할지를 결정하고, 보안을 유지하기 위해 사용됨.
대표적인 DCL 명령어로는 GRANT, REVOKE가 있음.

# MVC(Model-View-Controller)
>소프트웨어 디자인 패턴으로, 애플리케이션을 Model(데이터), View(사용자 인터페이스), Controller(데이터와 사용자 인터페이스 요소를 잇는 다리)으로 나누어 개발하는 방법. 모델과 뷰, 컨트롤러 간의 역할 분담으로 코드의 가독성과 유지보수성이 향상된다.

MVC정리 내용 참고
https://velog.io/@rmsqh4617/WIL-2%EC%A3%BC%EC%B0%A8

### 영속성
>데이터를 생성한 프로그램이 종료되어도 사라지지 않는 데이터의 특성을 말하며, 
JDBC, Spring JDBC, Persistence Framework 등을 사용하여 
데이터를 데이터베이스에 저장할 수 있다.

### ORM 사용 이유
>객체 지향 프로그래밍에서는 객체 간의 관계를 중요시하므로, 
ORM은 객체 간의 관계를 바탕으로 SQL을 자동으로 생성하여 불일치를 해결하고,
직관적인 코드로 비지니스 로직 집중 가능해진다.

### ORM 장단점
> <span style="color:blue">**장점**</span>
- 직관적인 코드 작성
- 재사용 및 유지보수 편리성 증가
- DBMS 종속성 저하

><span style="color:red">**단점**</span>
- ORM만으로는 완벽한 서비스 구현이 힘듦
- 프로시저가 많은 시스템에서는 객체 지향적인 장점을 활용하기 어려움
