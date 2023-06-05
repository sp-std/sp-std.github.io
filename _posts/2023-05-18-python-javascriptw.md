---
title: Python & javascript-01 (w/Chatgpt)
layout: post
date: '2023-05-18 19:46:17 +0900'
categories: jekyll update
---

**문제1.**        
길이가 같은 문자열 배열 my_strings와 이차원 정수 배열 parts가 매개변수로 주어집니다. parts[i]는 [s, e] 형태로, my_string[i]의 인덱스 s부터 인덱스 e까지의 부분 문자열을 의미합니다. 각 my_strings의 원소의 parts에 해당하는 부분 문자열을 순서대로 이어 붙인 문자열을 return 하는 solution 함수를 작성해 주세요.


**제한사항**       
- 1 ≤ my_strings의 길이 = parts의 길이 ≤ 100     
- 1 ≤ my_strings의 원소의 길이 ≤ 100     
- parts[i]를 [s, e]라 할 때, 다음을 만족합니다.     
- 0 ≤ s ≤ e < my_strings[i]의 길이     
	
	
```
** javascript
function solution(my_strings, parts) {
let answer = '';
for (let i = 0; i < my_strings.length; i++) {
	answer += my_strings[i].substring(parts[i][0], parts[i][1] + 1);
}
return answer;
}

** python
def solution(my_strings, parts):
	answer = ''
	for i in range(len(my_strings)):
			answer += my_strings[i][parts[i][0]:parts[i][1]+1]
	return answer**
```
<br><br>

**문제2.**      
길이가 같은 두 문자열 str1과 str2가 주어집니다.
두 문자열의 각 문자가 앞에서부터 서로 번갈아가면서 한 번씩 등장하는 문자열을 만들어 return 하는 solution 함수를 완성해 주세요.     


**제한사항**      
- 1 ≤ str1의 길이 = str2의 길이 ≤ 10
- str1과 str2는 알파벳 소문자로 이루어진 문자열입니다.
	
```
** python
def solution(str1, str2):
	answer = ''
	for i in range(len(str1)):
			answer += str1[i]+str2[i]
	return answer

** javascript
function solution(str1, str2) {
let answer = '';
for (let i = 0; i < str1.length; i++) {
	answer += str1[i] + str2[i];
}
return answer;
}
```

<br><br><br>
문제 출처 -[ 프로그래머스](https://programmers.co.kr/)
