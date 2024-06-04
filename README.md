# python

## In university i am learning python for basic open source project 
8week
### file input output

read() : 파일의내용을문자열로반환

readline() : 파일의한줄을읽어서문자열로반환

readlines(): 파일의모든줄을읽어서리스트로반환

전체파일을한번에처리해야하는경우read()를사용하고, 줄단위로처리해야하는
경우readline() 또는readlines()를사용

write() : 주어진하나의문자열을파일에작성

writelines() : 주어진문자열리스트를파일에작성

write()를사용할때줄바꿈문자(\n)을포함하면여러줄입력이가능하고,
문자열리스트를쓰려면writelines()를사용

import os 
os.path.exists()
---
#데이터 베이스 구축
1.데이터 생성
```
create table userTable(id char(4), userNamechar(15), email char(15), birthYearint);
Insert into userTableValues('john', 'john Bann', 'john@naver.com', 1990
```
2.데이터 뽑아내기
```
select id, birthyear from usertable where birthyear <=2000; #id, birthyear 열 뽑아내기
```
2.1 데이터 정렬
```
select * from usertable order by birthyear asc;
select * from usertable order by birthyear desc;
```

3. 파이썬에서 데이터 입력하는 코딩 순서
```
import sqlite3
con = splite3.connect()
cur = con.corsur() #실행,실행된 결과를돌려받는 커서
cur.execute("CREATE TABLE userTable (id char(4), userName char(15), email char(15), birthYear int)")
cur.execute("INSERT INTO userTable VALUES('john', 'John bann', 'john@naver,com', 1900)")
``` 

fetchone() 함수

는 파이썬의 데이터베이스 API에서 사용되는 함수 중 하나로, SQL 쿼리의 결과에서 한 행(row)을 가져오는 역할.
```
while True:
    row = cursor.fetchone()
    if row is None:
        break
    print(f'ID: {row[0]}, Name: {row[1]}, Age: {row[2]}')
```
---
맷플롯립

```
import matplotlib.pyplot as plt
plt.legend(loc= "upper.left') #왜 legend가 했더니 전설을 뜻하는 legend가아니고 '범례'를 뜻하는거
```
import numpy /// numpy란? 다차원 배열 객체와 배열을 다루는 다양한 함수를 제공

'k', 'r--', 'g' 그래프 색상 지정. k가 블랙인줄 몰랏음. 더 다양한 예시 추가예정.

np.random.randn(10) 크기가 10인 배열

plt.axis() x축 y축 범위 지정 ex) ``` plt.axis(0,10,0,20)```

