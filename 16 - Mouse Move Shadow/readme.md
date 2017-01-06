#Mouse Move Source 분석

## 목적

Mouse Move Shadow 소스 코드를 분석하고 어떤 메서드가 있는지 알아봄

## 새로운 개념 및 이벤트

### Event 내부의 this 와 e.target의 차이 

this는 해당 이벤트를 걸어준 엘리먼트를 의미하고 
e.target은 해당 이벤트가 발생하는 엘리먼트를 의미한다.

### 새로운 대입 방법

Object를 아래와 같은 형태로 바로 대입 가능 

```
  e = {
    offsetX : 3,
    offsetY : 4
  }

  let { offsetX: x, offsetY: y } = e;

  //3, 4 출력됨 
  console.log(x,y)
```

### Math

javascript 수학 관련된 함수들 집합 

참고 : http://www.w3schools.com/jsref/jsref_obj_math.asp