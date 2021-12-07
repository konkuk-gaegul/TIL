# 파이썬 문제 풀이



## 		짝수 / 홀수 더하기

### for 

n = int(input())

for i in range(1, n+1)

​	if i % 2: continue

​	else : total += i

print(total)



### range

n = int(input())

sum( range(0, n+1, 2))



## 		16진수 구구단

n = int( input(), base = 16)

for i in range(1, 16):

​	print( f'{n:X}*{i:X}={n*i:X}' )

## 		10진수 구구단

for i in range(2, 10):

​	for j in range(1, 10):

​		print( f' {i*j} ', end = ' ' ) or print(' {}  '.format(i*j))

​	print( ' ')



## 		등차, 등비 수열

a,  d, n = map(int, input().split())

for i in range(n-1)

​	a = a + d

## 	별 찍기 (n=5)

'''

for i in range(n): 	   	or in range(1,n+1)

​	for j in range(i+1): 	or in range(i)

​		print('*', end = '')

​	print()

'''

for i in range(n):

​	 for j in range(i+1):

​	  print('*',end='')

 print()

'''

for i in range(n, 0, -1):

​	 for j in range(i):

​	  print('*',end='')

​	 for k in range(n-j):

​	  print(' ',end='')

 print()

'''

for i in range(n,0,-1):

 	for j in range(n-i):

  		print(' ',end = '')

 	for k in range(i):

 		 print('*',end='')

 print()

'''

for i in range(n):

​	 for k in range(n-i, 0, -1):

​	  print(' ',end='')

​	 for j in range(0, 2*i+1):

​	  print('*',end='')

 print()

'''

## 	2차원 리스트

n = int(input())

a = list( map(int, input().split()))

check = [0]*24

for i in a:

​	check[i] += 1

print(*check, end='')

'''

for i in range(n):

​	 check[ a[i] ] += 1 

for j in range(1, 24):

​	 print( check[j], end=' ')

'''

























