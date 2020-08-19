---
layout: post
title:  "Join 개념 및 종류"
summary: 공공데이터 인턴 교육
author: 서준석
date: '2020-08-19 12:31:00 +0530'
category: database
thumbnail: /assets/img/products/dbsql/join.png
keywords: database, nia, sql, join
permalink: /blog/database_join
---
# Join

## 1. 개념
* 조인은 관계형 DB에서 가장 기본적이고 중요한 기능
* 집합간의 곱
* 관계형 DB에서는 서로 독립적인 Data들간의 정보연결을 위해 Join을 이용해 필요 시 다양한 정보를 참조하고 창출
* 연산자에 따라 Equi Join, Non-Equi Join, Anti Join 등 다양

### 필요성
* Data 중복 제거
* 여러 Entity로 Data가 나눠서 저장
* 연결 관계를 통해 여러 Entity의 Data를 조회

## 2. 종류
1. Natural Join
    * 두 테이블에서 Data 유형과 이름이 일치하는 열을 기반으로 자동으로 테이블을 Join, ANSI 표준
    * Join은 두 테이블의 이름과 Data 유형이 동일한 열에서만 발생
    * 둘 중 하나라도 다를 경우 Natural Join 구문에서 오류 발생
2. Equi Join
    * 등호 연산자가 포함된 Join 조건이 있는 Join
    * 지정 열에 동등 값이 있는 행을 결합
3. Non-Equi Join
    * <= 및 >= 등의 범위 조건을 이용한 Join
4. Outer Join
    * Outer Join 대상 Table의 자료가 존재할 경우 그 정보를 출력하고 없으면 기존 자료만 출력
    * 한쪽 집합이 기준이 되어 다른 쪽 집합의 연결되는 조건에 상관없이 기준이 되는 집합은 무조건 추출되는 조인
    * Outer Join의 기준이 되는 집합은 항상 Join에 성공
    * 종류
        1. Left Outer Join
        2. Right Outer Join
        3. Full Outer Join  