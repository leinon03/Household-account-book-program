기존의 가계부 프로그램은 객관적인 분석의 어려움과 실제 사용되는 기능의 한정성이라는 한계를 가지고 있었습니다.
저희 3팀은 이러한 문제를 해결하기 위해, 개인의 수입/지출 내역을 체계적으로 관리하고 시각적으로 소비 패턴을 파악할 수 있는 새로운 가계부 프로그램을 개발했습니다.

본 프로그램을 사용하기 위해서는 데이터베이스로 MySQL 설치가 필수입니다.

프로그램 실행 전, 데이터베이스를 생성하고 테이블을 설정해야 합니다.
데이터베이스 : udb  
테이블 : client, maindb

데이터베이스 테이블의 상세 구조는 다음과 같습니다.

테이블 이름 | 필드 (Field) | 데이터 타입 (Type) | NULL 허용 (NULL) | 제약 조건 (Key) | 상세 설정

udb
client (사용자 정보) | ID | varchar(10) | (NOT NULL) | PRI (Primary Key)  
password | varchar(20) | (NOT NULL)

maindb
id | int | (NOT NULL) | PRI (Primary Key) | AUTO_INCREMENT  
client_id | varchar(50) | (NOT NULL)  
date | date | (NOT NULL)  
type | varchar(20) | (NOT NULL)  
category | varchar(50) | (NULL)  
title | varchar(100) | (NULL)  
amount | int | (NOT NULL)  

테이블 구조에 대한 더 자세한 정보는 첨부된 JPG 파일을 참고해 주세요.

다운로드받은 프로그램 내의 LedgerDB 및 UserDB 파일에서 현재 사용 중인 MySQL의 데이터베이스 ID와 비밀번호를 자신의 환경에 맞게 수정한 후 프로그램을 실행하십시오.

프로그램 사용이나 설치 중 궁금한 사항이 있다면 언제든지 아래 이메일로 문의해 주세요.
문의처: chb9929@sunmoon.ac.kr
