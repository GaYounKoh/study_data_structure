# study_data_structure
study_data_structure
<br>
<br>
[Tips]
* def 줄 빼고 다 지워도 됨.
문제에서
* <span style = 'color:red'>~인지 아닌지</span> 확인하라고 했으면 <span style = 'color:red'>[return 조건문]</span>.
* <span style = 'color:red'>출력</span>하라고 했으면 <span style = 'color:red'>print</span>.
* 단순히 <span style = 'color:red'>반환</span> 하라고 했으면 <span style = 'color:red'>[return 코드]</span>만, print하면 안됨.

<br>
<br>

[문자열 안에 따옴표 넣기](https://blog.hexabrain.net/275) <br>

<br>

``` python
from IPython.core.interactiveshell import InteractiveShell
InteractiveShell.ast_node_interactivity = "all"
```
<br>

# 220319 rank (solved Q, score)
89396 (6) <br>
87956 (7, 1016) <br>

<br>

# 220321 rank (solved Q, score)
77424 (8, 1025) <br>
<br>

# 3w 데이터 마이닝
* 3w 수업내용 : greedy (그리디)
1. 거스름돈
2. 1이 될때까지
3. 곱하기 혹은 더하기
4. 모험가 길드 문제

--
* 3w 실습
1. 주식 매매 최대이득
2. 아이에게 원하는 쿠키 주기
<br>

# 220322 rank (solved Q, total score)
74820 (9, 1028) <br>
<br>


# 220324 rank (solved Q, total score)
72352 (10, 1031) <br>
<br>

# 220325 rank (solved Q, total score)
67743 (11, 1037) <br>
60415 (12, 1049) <br>
58852 (13, 1052) <br>
<br>

# 220327 rank (solved Q, total score)
55131 (14, 1060) <br>
<br>

# 220328 rank (solved Q, total score)
데이터 마이닝 시간에 한 문제 풀었음. (교수님 풀이 보기 전에 주신 시간 (15분)내에 풀었음.) <br>
52129 (15, 1067) <br>
<br>
[교수님께서 참고하신 듯한 자료...](https://doing7.tistory.com/70) <br>
<br>

# 220330 rank (solved Q, total score)
50339 (16, 1072) <br>
<br>

# 220401 rank (solved Q, total score)
50080 (17, 1073) <br>
요새 점수 잘 받다가 갑자기 1점 받으니까 좀 기부니가 좀 그르네,,, - 자릿수별로 나눠서 더하는 방법이 있었다니... <br>
<br>

46910 (18, 1082) <br>
... 완전탐색은 구현문제.. 시간에 구애받지 않음. 문제나 잘 읽을 것... <br>
나도 진짜 잘 풀었는데 딕셔너리 아닌 리스트로 푸는 방법도 있었음. <br>
<br>

43122 (19, 1094) <br>
PaGe 3 ClEaR!!~!~!!~!!!!
<br>
42265 (20, 1097) <br>
아... 다른 사람들 풀이보니까 조건에 메여있을게 아니라 조건을 적절히 활용할 줄 알았어야... <br>
3000번이 아니라 그냥 n번만 돌리는 방법이.... 그치... <br>

# 220402 rank (solved Q, total score)
40348 (21, 1104) <br>
ord라는 함수에 대해 알아볼것,,,,(~~문자열 순서대로 만드는 함수인듯,,,~~ 알파벳 순서 반환) <br>
<br>

39858 (22, 1006) <br>
어제 약수 문제 풀었던 기억이 남아있었고, 시간제약이 없었어서 막힘 없이 풀어버림... <br>
(근데 이중 for loop에 for loop 하나 더는 좀 심하긴 했음.) <br>
<br>

39593 (23, 1007) <br>
다른 사람 풀이 보고 나는 대체 그 생각에 접근까진 해놓고 왜 이렇게 푼 걸까 싶었음. <br>
<br>

39338 (24, 1008) <br>
다른 사람 풀이 보니까 -일 때, +일 때로 나눠서 하는게 좋을 것 같음. <br>
<br>

# 220404 5w 데이터 마이닝
꺅 스택문제를 풀었다?!?!?!?!?!?!!!!!?!?!? 세상에. 심지어 혼자 풀었다????!?!?!?! <br>
그런데 오늘 수업 많이 졸았음... 킹킹,,~ <br>
<br>

* ***스택*** <br>
1. <span style = 'color:red'>후입 선출</span> (선입 후출, LIFO) <br>
a. 기억하고 있어야 할 때 <br>
b. 가장 ***최근***에 들어오는게 ***가장 먼저*** 나가야할 때 씀. <br>
c. ***후입***일 수록 ***우선순위***가 높음. (가장 ***마지막***에 들어온 원소를 <span style = 'color:red'>***top***</span>이라고 부름.) <br>
d. 입구, 출구 하나 <br>
<br>

2. 예시 <br>
```python
stack = []

## 스택 처리 코드
stack.append(5) # stack 상태 : [5]
stack.append(2) # stack 상태 : [5,2]
stack.append(3) # stack 상태 : [5,2,3]
stack.append(7) # stack 상태 : [5,2,3,7]
stack.pop()     # stack 상태 : [5,2,3]    # 가장 나중에 들어온 7이 삭제 됨.
stack.append(1) # stack 상태 : [5,2,3,1]
stack.append(4) # stack 상태 : [5,2,3,1,4]
stack.pop()     # stack 상태 : [5,2,3,1]  # 가장 나중에 들어온 1이 삭제 됨.

## 결과
stack = [5,2,3,1]
```
<br>

3. tips <br>
a. 못하겠으면 손으로 먼저 풀어보기! <br>
b. pop()은 뽑아서 삭제하는 코드 <br>
c. <span style = 'color:red'>***[-1]로 인덱싱***</span> 해서 마지막 꺼 뽑아서 ***조건검사*** 하는 것도 잊으면 안됨. <br>
d. 짝 맞춰야하는 문제는 dic에 짝 지어주는게 핵심. <br>
--- <span style = 'color:red'>{후입:선입}</span>식으로, <br>
key로 value 찾는 기능 이용. <br>
e. stack은 연산을 효율적으로 하기 위해 하는 것. (속도 면...) <br>


<br>

* ***큐*** <br>
1. 선입선출 (FIFO) <br>
들어온 순서 그대로 기억해야할 때 <br>
a. 입구, 출구 각각 <br>
<br>

2. BFS 문제에서 활용 <br>
<br>

3. queue 구현을 위한 라이브러리 (.pop(0) 성능이 나쁘기 때문에 사용.)
```python
from collections import deque

queue = deque(list) # 이런식으로 받아서 사용.

## .pop(0)대신 .popleft() 사용. 성능 훨씬 좋음.
```
<br>

# 220406 rank (solved Q, total score)
37447 (25, 1116)
* 소수 찾기문제 <br>
원 풀이법: 에라토스테네스의 체 <br>
응용한 풀이법: 배수를 계속 차집합 <br>

# 220407 rank (solved Q, total score)
37331 (26, 1117)
* list에서도 index 쓰임.
<br>

# 220410 rank (solved Q, total score)
36683 (27, 1120) <br>
for loop 돌리다가 다 돌기 전에 먼저 조건 만족하면 그냥 리턴 하는... <br>
<br>

# 220411 6w 데이터 마이닝
* ***dfs*** 깊이 우선 탐색 <br>
1. 모두방문 <br>
a. 재귀함수

그니까,, 뭔가 질문을 전혀 또 안꼬아서 하시니까... 내가 생각한 대답이 오답일까봐 답을 못하겠던 날이었...
<br>

# 220417
while 옆에는 종료 조건임. 조건 불충족시 종료됨.
<br>

# 220426
36894 (28, 1122) <br>

# 220430
24799 (29, 1132) <br>

# 220507
34502 (30, 1135) <br>

## strip은 덮어쓰기가 안됨.
좌우 '.' 지우기가 됨. <br>
<br>

## filter 함수 <br>
내장함수를 built in 함수라고 함. <br>
filter 대신 for loop의 enumerate 사용 가능. <br>
* 2개 이상의 문자에 대해서는 인덱싱이 안됨. <br>
[참고1](https://ai-hyu.com/python-%ED%8C%8C%EC%9D%B4%EC%8D%AC-%EB%A6%AC%EC%8A%A4%ED%8A%B8-%EC%9D%B8%EB%8D%B1%EC%8A%A4-%EC%97%AC%EB%9F%AC%EA%B0%9C-%EC%B0%BE%EA%B8%B0/) <br>
[참고2 - 딱 필요한 부분만 적혀있음.](https://weejw.tistory.com/374) <br>
[참고3 - 자세한 설명](https://bill1224.tistory.com/228) <br>


sub라는 함수가 있었음. <br>
정규식이라는게 있었음... (re 모듈을 사용하는...) <br>
> re 모듈은 Regular Expressions의 약어 <br>
(뭔가 당장은 몰라도 될 것 같은 느낌... 이상한 문자들이 코드인듯., 수준 내에서는 충분히 잘 풀었음.) <br>

