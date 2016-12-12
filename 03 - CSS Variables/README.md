#Clock Source 분석

## 목적

아날로그 시계처럼 동작하도록 구현한다.

## 새로운 개념 및 이벤트

### :root
  문서 구조에서 root요소에 적용함.
  변수형태로 사용 가능

  선언은 prefix '--' 를 사용함.
  var를 이용해 가져 올 수 있음.


  ```
  :root{
    --bgcolor: #654344;
  }

  body{
    color: var(--bgcolor);
  }

  ```

  참고 : https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_variables

### dataset
  HTMLElement.dataset 를 통해서 해당엘리먼트의 'data-'인 커스텀 엘리먼트의 값을 map형태로 가져올 수 있음.

  참고 : https://developer.mozilla.org/ko/docs/Web/API/HTMLElement/dataset

### document.documentElement.style.setProperty
  해당 element에 css 속성을 부여 할 수 있다.

  ```
  setProperty(propertyname, value, priority) throws DOMException;
  ```