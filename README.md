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
