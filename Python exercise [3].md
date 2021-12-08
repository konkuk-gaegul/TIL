# 파이썬 실습

## 	숫자의 개수

A = 150 / B = 266 / C = 427

solve = A*B*C

solve = list(map(int, str(solve)))

ans = [0]*10

for i in solve:

 ans[i] = ans[i] + 1

print(ans, sep = '\n')

'''

## 	최소 / 최대

n = int(input())

a = list( map( int, input().split()))

mini = 1000001

maxi = -1000001

for x in a:

 if mini > x: mini = x

 if maxi < x: maxi = x

print(mini, maxi )

'''

## 	나머지 개수 (***)

n = 1

ans = [0]*42

for _ in range(n):							%% n번 반복한다

 n = int(input())

 i = n % 42

 ans[i] = 1

print(sum(ans))

'''

## 	바둑알 놓기

a = [  [0]*5 for _ in range(5)  ]		%%  list comprehension

n = int( input())

for _ in range(n):							%% n번 반복한다

 i, j = map(int, input().split())

 a [i-1] [j-1] = 1

for row in a:

 for col in row:

  print(col, end = ' ')

 print()

'''

## 	십자 뒤집기

a = [ list(map(int, input().split())) for _ in range(19)]

n = int(input())

x, y = map(int, input().split())

for i in range(19):

 if i != x-1:

  if a[i][y-1] == 0: a[i][y-1] = 1

  elif a[i][y-1] == 1: a[i][y-1] = 0

for j in range(19):

 if j != y-1:

  if a[x-1][j] == 0: a[x-1][j] = 1

  elif a[x-1][j] == 1: a[x-1][j] = 0

for row in range(a):

 for col in range(row):

  print(col, end = ' ')

 print()

'''

## 	별 찍기 1번 (****)

n = 5

a = [ ['']*n for _ in range(n) ]

\#조건에 맞는 곳에 '*' 입력

for i in range(n):

 for j in range(i+1):

  if j <= i:

   a[i][j] = '*'

\#변경된 리스트 a를 행렬에 맞게 출력

for i in range(n):

 for j in range(n):

  print(a[i][j], end='')

 print()



















