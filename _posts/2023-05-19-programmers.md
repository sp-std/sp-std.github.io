---
title: 파이썬 문법 메모
layout: post
date: '2023-05-19 16:52:42 +0900'
categories:
- jekyll
- update
---

반복적으로 나오는 기본 메서드들은 확실히 기억해 놓자. (자료형으로 나눠서 메서드들을 기억하는 게 좋을 것 같다)

**문자형**은 immutable 자료형 > 슬라이싱으로 처리, 내용을 변경할 수 없다.<br>
**리스트**, **딕셔너리**, **집합형**은 mutable 자료형<br>
**문자형**, **리스트**, **딕셔너리**는 시퀀스 자료형<br>
<br>
```
문자열.split(sep=구분자, maxsplit=분할횟수) > 리스트로 반환
리스트.append()
리스트.insert
리스트.sort(opt(reverse=True)) > 원본값 변경
sorted(리스트) > 새로운 리스트 반환
' '.join(리스트) 
문자열.replace('A', 'B') / 연결해서 사용 가능
strip() > 공백 제거, 문자 제거
del 리스트
리스트.remove()
리스트.pop()
문자열.find()
문자열.rfind()
리스트 나누기 > 리스트[start:end:split]
arr = [[0] * n for _ in range(n)]
range(start, stop, step)
.count()
round(num, digit)
```
<br>
한번 더 풀어볼 것.

- 배열의 원소만큼 추가하기
- 문자열 바꿔서 찾기
- 꼬리 문자열
- 0 떼기 (break)
- l로 만들기<br>
replace는 새로운 문자열 반환, 슬라이싱으로 처리하자
- 할 일 목록<br>
zip() 함수는 이터레이터를 반환, 인덱스 사용이 불필요. 언패킹 활용 가능
- 주사위 게임2
- 배열의 원소 삭제하기
- 가까운 1 찾기
- 특별한 이차원 배열1,2
- 9로 나눈 나머지
- 그림확대
- 배열만들기 2
- 배열만들기 4
- 배열만들기 6
- 수열과 구간 쿼리
- 주사위 게임 3 (딕셔너리 자료형 활용)
<br>
