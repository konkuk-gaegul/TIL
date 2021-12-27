# 코딩 테스트 연습 [1]

## 유클리드 호제법

두 수의 최대공약수를 구해보자

```
a, b = map(int, input().split())

if b > a:

  a, b = b, a

while True:

  n = a % b
  a, b = b, n

  if n == 0: break
  
print(f'최대공약수는 {a}입니다.')
```

```
10 9
최대공약수는 1입니다.
```



## power() 함수 작성하기

n이 주어졌을 때, 2^n을 구하는 함수를 작성해보자

함수의 리턴 값은 2^n 값

```
n = int(input())

def power(n):
  
  return 2**n
```

```
power(3)
8
```



## n^m 구하기

임의의 정수 n, m이 주어졌을 때,

n^m = n(1) * n(2) * n(3) *...* n(m)

```
n, m = map(int, input().split())
p = n

while m:

  m = m-1
  p = p*n
print(p)
```

```
2 3
16
```



## 러시아 농부(?)의 곱셈

왼쪽의 수는 2로 나눠주고, 나머지는 버린다. (1이 될 때 까지 반복)

오른쪽에 있는 수는 두 배 해준다.

왜 이런..곱셈을..

```
n, m = map(int, input().split())
p = m

while n != 1:
  n = n//2
  m = m*2
  print(n, m)

  if n%2 == 1:
    p += m

print(p)
```

```
123 12
61 24
30 48
15 96
7 192
3 384
1 768
1476
```



## 팩토리얼 구하기

```
n = int(input())
m = n-1

for _ in range(n-1):
  n = n*m
  m = m-1
print(n)
```

```
5
120
```







































