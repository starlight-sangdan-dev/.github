# .github
별빛상단 공식 Github

# 코딩 스타일 가이드
이 문서는 코드 작성 시 따라야 하는 코딩 스타일 가이드에 대해 설명합니다. 아래의 규칙을 따라 코드를 작성하면 코드의 가독성과 일관성을 유지할 수 있습니다.

## 세미 콜론
* 모든 구문의 끝에는 ;(세미콜론)을 사용합니다.

## 이름 짓기
* 컴퓨터 또는 수학에서 사용하는 개념들을 제외하고 약어를 사용하지 않습니다. 컴퓨터 또는 수학에서 사용하는 개념들의 약어를 썼다면 주석에 어떤 약어인지 표현합니다.

## 상수 명명 규칙
* 상수는 모두 대문자로 작성합니다.
* 단어 사이를 밑줄(_)로 구분합니다.

### 타입스트립트

```typescript
const MAX_VALUE: number = 100;
const DEFAULT_TIMEOUT: number = 5000;
```

### C++

```c++
const int MAX_VALUE = 100;
const int DEFAULT_TIMEOUT = 5000;

```

## 변수 명명 규칙
* 변수는 카멜 표기법을 사용합니다.
* 첫 번째 단어는 소문자로 시작하고, 이후의 각 단어의 첫 글자는 대문자로 작성합니다.

### 타입스트립트

```typescript
let firstName: string = "John";
let maxValue: number = 10;
let defaultTimeout: number = 3000;
```
### C++

```c++
int age = 25;
double totalPrice = 59.99;
string firstName = "John";
```

## 함수 명명 규칙
* 함수는 파스칼 표기법을 사용합니다.
* 각 단어의 첫 글자는 대문자로 작성합니다.

### 타입스트립트

```typescript
function calculateSum(a: number, b: number): number {
  return a + b;
}

function getUserInfo(userId: string): UserInfo {
  // ...
}

function isValidInput(input: string): boolean {
  // ...
}
```

### C++

```c++
int CalculateSum(int a, int b) {
  return a + b;
}

string GetFullName(string firstName, string lastName) {
  // ...
}

bool IsValidInput(string input) {
  // ...
}
```

## 인터페이스 명명 규칙

* 인터페이스는 파스칼 표기법을 사용합니다.
* 각 단어의 첫 글자는 대문자로 작성합니다.

### 타입스트립트

```typescript
interface IUserInterface {
  // ...
}

interface ILogger {
  // ...
}

interface IDataProvider {
  // ...
}
```


## 클래스 명명 규칙

* 클래스는 파스칼 표기법을 사용합니다.
* 각 단어의 첫 글자는 대문자로 작성합니다.
  
### 타입스트립트

```typescript
class UserManager {
  // ...
}

class DatabaseConnector {
  // ...
}

class FileReader {
  // ...
}
```

### C++

```c++
class UserManager {
  // ...
};

class DatabaseConnector {
  // ...
};

class FileReader {
  // ...
};
```



## 띄어쓰기 규칙

* 들여쓰기는 2칸을 사용합니다.
* 산술 연산자, 할당 연산자, 비교 연산자, 논리 연산자 주변에는 공백을 추가합니다.


### 타입스트립트

```typescript
let result = a + b;
if (x > 0 && y < 10) {
  // ...
}
```

### C++

```c++
int result = a + b;
if (x > 0 && y < 10) {
  // ...
}

```


## 줄바꿈 규칙
* 함수나 메서드의 파라미터가 3개 이상인 경우, 콤마 이후에 줄을 바꿉니다. 한 줄에 파라미터 하나씩 작성합니다.
* 중괄호는 열고 바로 줄을 바꿉니다.


### 타입스트립트

```typescript
function exampleFunction(
  param1: number,
  param2: string,
  param3: boolean,
  param4: string[]
): void {
  // ...
}

class ExampleClass {
  constructor() {
    // ...
  }

  methodWithLongParameterList(
    param1: number,
    param2: string,
    param3: boolean,
    param4: string[]
  ): void {
    // ...
  }
}
```

### C++

```c++
void ExampleFunction(
    int param1,
    double param2,
    string param3
) {
  // ...
}

class ExampleClass {
public:
  ExampleClass() {
    // ...
  }

  void MethodWithLongParameterList(
      int param1,
      double param2,
      string param3
  ) {
    // ...
  }
};

```

## 중괄호 규칙

* 중괄호를 열 때는 같은 줄에 작성합니다.
* 코드가 한 줄만 있더라도 중괄호를 사용합니다.

### 타입스트립트

```typescript
if (condition) {
  // ...
}

while (condition) {
  // ...
}

function exampleFunction() {
  // ...
}

class ExampleClass {
  method() {
    // ...
  }
}
```
### C++

```c++
if (condition) {
  // ...
}

while (condition) {
  // ...
}

void ExampleFunction() {
  // ...
}

class ExampleClass {
  void Method() {
    // ...
  }
};

```

## 주석 사용 규칙
* 필요에 따라 주석을 사용하되, 코드의 의미나 의도를 주석으로 표시하는 것보다 함수명이나 변수명에 명확한 의미를 부여하는 것이 좋습니다.
* 필요에 따라 // TODO, 참고 링크, 일시적인 주석 등을 사용할 수 있습니다.
