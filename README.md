# sum-test
- 인자를 주면 그 값까지 더하는 알고리즘
- O(1) 로 만들기 위해 n(n+1+/2
  
### main.cpp
- sum함수에 인자값으로 10을 주면 1부터 10까지의 합을 구한다.
```
// main.cpp
#include <stdio.h>
#include "sum.h"

int main() {
  int s = sum(10);
  printf("result=%d\n", s);
}
```

### sum.cpp
- sum 함수를 선언한다.
- sum 함수는 n까지의 합을 구하는 함수.
``` 
// sum.cpp
#include "sum.h"

int sum(int n) {
	return n*(n+1)/2;
}
```

### sum.h
- 함수를 먼저 정의하고 있다.
```
// sum.h
#pragma once

int sum(int n);
```
### Makefile

