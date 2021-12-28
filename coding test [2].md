# 코딩 테스트 스터디 [2]

## 피보나치 수 1

리스트를 이용하여 구해보자

0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, ...

```
n = 10

i = [0, 1]

for j in range(2, n+1):
  
  i.append( i[j-1] + i[j-2] )

print(i[j])
```

j가 range안에서 0부터 시작하면 list out of range가 발생한다.

따라서 range(2, n+1)로 보정하여 i.append( i[j-1] + i[j-2])로 보정했다.

```
55
```



## 피보나치 수 2

리스트 제외 다른 방법으로 접근해보자

### 함수와 반복문 사용

```
def pivo(n):

  i, j = 0, 1

  for _ in range(n):
    
    i, j = j, i+j

  return i
```









































