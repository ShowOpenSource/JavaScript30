#Array Source 분석

## 목적

Array의 새로운 함수들을 사용해본다.

## 새로운 개념 및 이벤트

### Array

  * some()
    배열 요소 중에서 하나라도 특정 조건을 만족하는지 확인하는 메서드
    function([배열 요소 값],[배열 요소 위치],[현재 돌고 있는 배열 자체])

    출처 : http://programmingsummaries.tistory.com/357

  * every()
    배열의 모든 요소가 특정 조건을 만족하는지 알고 싶을때 사용하는 메서드
    function([배열 요소 값],[배열 요소 위치],[현재 돌고 있는 배열 자체])

    출처 : http://programmingsummaries.tistory.com/357

  * find()
    해당 배열 안의 값을 하나 반환
    이 때, 콜벡으로 전달받은 테스트 함수가 요구하는 조건을 만족하는 값을 반환

    출처 : https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array/find

  * findIndex()
     테스트 함수를 만족하는 배열의 첫 번째 요소에 대한 인덱스를 반환
     그렇지 않으면 -1이 리턴

     출처 : https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex

  * splice()
    어떤 배열의 일부에 대한 얇은 복사본 배열을 반환
    function([begin][end])




#### tip) slice를 이용하여 배열의 중간값 삭제하기

배열.splice(인덱스,1);
//리턴값은 삭제된 배열 요소이다.
//배열 자체는 이제 삭제한 요소를 제거한 요소들로만 구성되어 있다.

삭제할 요소의 인덱스는 0부터 시작된다는 점만 주의하면 사용에 큰 어려움은 없다. 다음은 간단한 사용예이다.

var array = [0, 1, 2, 3, 4, 5];

array.splice(2, 1);

//array에는 세번째 요소가 빠진 상태가 된다.
[0, 1, 3, 4, 5]

출처 : http://programmingsummaries.tistory.com/140