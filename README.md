# ⏰ 21시 캠프 입구 집합! ⏰

# MySQL_Study 
프로그래머스의 MySQL 문제 푸는 스터디 입니다.<br>
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)


## 규칙
１. 하루에 두 문제씩 풀어오기. </br>
１. 자기 이름으로 된 브런치의 자기 이름으로된 레포지토리에 날짜별로 저장하기 </br>
１. 중도 포기 시, **슬랙에 이름 박제** </br>

**브런치 하고, 자기 이름 디렉토리에 저장**

## 멤버

[최혁](https://github.com/Youkamii)  [안태인](https://github.com/TAENNOS)  [고광주](https://github.com/KoKwangJu)  [이예진](https://github.com/dlwls423)  [임지훈](https://github.com/vanillacake369) [정성호](https://github.com/jshstar) [진유록](https://github.com/jinyr1128) [김영규](https://github.com/hana2set) [김종규](https://github.com/Kim-Jong-Gyu) [조원호](https://github.com/wonowonow) [문정현](https://github.com/JungHyunMoon) [창다은](https://github.com/de123456sdf) [이지선](https://github.com/jiisuniui)

<div align = "center">
  
![납치된거야](https://github.com/Youkamii/MySQL/assets/87900502/a2decd9e-9dde-42fd-802e-3378f04f94a3)

 **❝ 너 납치된거야  ❞**

</div>

---
### 기본 SQL?<br>
1.SELECT: 데이터베이스에서 데이터를 조회하는 데 사용됩니다. 특정 테이블에서 하나 이상의 열을 선택하여 결과를 반환합니다.<br>
`SELECT column1, column2 FROM table_name;`<br><br>
2.WHERE: SELECT 쿼리에 조건을 추가하여 특정 기준에 맞는 데이터만 조회합니다.<br>
`SELECT column1, column2 FROM table_name WHERE condition;`<br><br>
3.JOIN: 두 개 이상의 테이블을 결합하여 관련된 데이터를 조회합니다. 주로 테이블 간의 관계를 기반으로 사용됩니다.<br>
- INNER JOIN: 두 테이블 모두에서 일치하는 데이터만 반환합니다.<br>
`SELECT table1.column1, table2.column2 FROM table1 INNER JOIN table2 ON table1.common_column = table2.common_column;`<br><br>
- LEFT JOIN: 왼쪽 테이블의 모든 데이터와 오른쪽 테이블의 일치하는 데이터를 반환합니다. 오른쪽 테이블에 일치하는 데이터가 없는 경우 NULL을 반환합니다.<br>
`SELECT table1.column1, table2.column2 FROM table1 LEFT JOIN table2 ON table1.common_column = table2.common_column;`<br><br>

4.GROUP BY: 데이터를 그룹화하여 집계 함수(예: COUNT, MAX, MIN, SUM, AVG 등)를 사용할 때 유용합니다.<br>
`SELECT column1, COUNT(*) FROM table_name GROUP BY column1;`<br><br>
5.ORDER BY: 조회 결과를 특정 열에 따라 정렬합니다. 기본적으로 오름차순으로 정렬되며, DESC 키워드를 사용하여 내림차순으로 정렬할 수 있습니다.<br>
`SELECT column1, column2 FROM table_name ORDER BY column1 DESC;`<br><br>
6.INSERT INTO: 새로운 데이터를 테이블에 삽입합니다.<br>
`INSERT INTO table_name (column1, column2) VALUES (value1, value2);`<br><br>
7.UPDATE: 기존 데이터를 수정합니다.<br>
`UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;`<br><br>
8.DELETE: 테이블에서 데이터를 삭제합니다.<br>
`DELETE FROM table_name WHERE condition;`<br><br>
9.LIMIT: SELECT 문을 사용할 때 결과의 수를 제한합니다. 페이징 처리에 유용합니다.<br>
`SELECT * FROM table_name LIMIT 10; -- 처음 10개의 결과만 반환`<br><br>
10.OFFSET: LIMIT와 함께 사용되어, 어느 지점부터 데이터를 가져올지 지정합니다.<br>
`SELECT * FROM table_name LIMIT 10 OFFSET 5; -- 6번째부터 10개의 결과를 가져옴`<br><br>
11.LIKE와 WILDCARDS: 문자열 검색에 사용되며, %와 _ 와일드카드 문자와 함께 사용됩니다.<br>
- %는 0개 이상의 문자를 나타냅니다.
- _는 정확히 하나의 문자를 나타냅니다.
  `SELECT * FROM table_name WHERE column LIKE 'a%'; -- 'a'로 시작하는 모든 데이터 검색`<br><br>

12.AS: 열이나 테이블에 별칭을 지정합니다. 복잡한 쿼리에서 가독성을 높이는 데 유용합니다.<br>

`SELECT column1 AS c1, column2 AS c2 FROM table_name;`<br><br>

13.DISTINCT: 중복된 값을 제거하고 고유한 값만 반환합니다.<br>

`SELECT DISTINCT column1 FROM table_name;`<br><br>

14.COUNT, MAX, MIN, AVG, SUM: 집계 함수를 사용하여 데이터 그룹에 대한 통계 정보를 얻습니다.<br>

`SELECT COUNT(column1), MAX(column2) FROM table_name;`<br><br>

15.HAVING: GROUP BY와 함께 사용되어 그룹화된 데이터에 조건을 적용합니다.<br>

`SELECT column1, COUNT(*) FROM table_name GROUP BY column1 HAVING COUNT(*) > 5;`<br><br>

16.UNION과 UNION ALL: 두 개 이상의 SELECT 쿼리 결과를 결합합니다. UNION은 중복을 제거하고, UNION ALL은 모든 결과를 포함합니다.<br>

`SELECT column1 FROM table1 UNION SELECT column1 FROM table2;`<br><br>

17.INDEXES: 데이터 검색 성능을 향상시키기 위해 인덱스를 생성하거나 관리합니다.<br>

`CREATE INDEX idx_column1 ON table_name (column1);`<br><br>

---


## 진행 회차

| 회차               | 문제                                                                                                                                                                                                                                  |   |
|------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---|
| 1회차(2023.12.06)  | [아픈 동물 찾기](https://school.programmers.co.kr/learn/courses/30/lessons/59036), [중복 제거하기](https://school.programmers.co.kr/learn/courses/30/lessons/59408)            |   |
| 2회차(2023.12.07)  | [어린 동물 찾기](https://school.programmers.co.kr/learn/courses/30/lessons/59037), [동물의 아이디와 이름](https://school.programmers.co.kr/learn/courses/30/lessons/59403)            |  👈 |
| 3회차(2023.12.08)  | [여러 기준으로 정렬하기](https://school.programmers.co.kr/learn/courses/30/lessons/59404), [동물 수 구하기](https://school.programmers.co.kr/learn/courses/30/lessons/59406)            |   |
| 4회차(2023.12.11)  | [최솟값 구하기](https://school.programmers.co.kr/learn/courses/30/lessons/59038), [이름이 있는 동물의 아이디](https://school.programmers.co.kr/learn/courses/30/lessons/59407)            |   |
| 5회차(2023.12.12)  | [역순 정렬하기](https://school.programmers.co.kr/learn/courses/30/lessons/59035), [상위 n개 레코드](https://school.programmers.co.kr/learn/courses/30/lessons/59405)            |   |


