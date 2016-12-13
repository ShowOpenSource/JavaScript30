#Array Source 분석

## 목적

Array의 새로운 함수들을 사용해본다.

## 새로운 개념 및 이벤트

### Array

	* filter()
		콜백 함수에 지정된 조건을 충족하는 배열의 요소를 반환합니다.        
        출처 : https://msdn.microsoft.com/ko-kr/library/ff679973(v=vs.94).aspx
        
	* map()
        배열의 각 요소에 대해 정의된 콜백 함수를 호출하고 결과가 포함되어 있는 배열을 반환합니다.        
        출처 : https://msdn.microsoft.com/ko-kr/library/ff679976(v=vs.94).aspx
    * sort()
        정렬
		sort 안의 함수 의 동작 원리  
        function compare(a, b) {
          if (a 가 b 보다 작은 순서 지정 기준) {
            return -1;
          }
          if (a가 b보다 큰 순서 지정 기준) {
            return 1;
          }
          // a와 b 가 같은 경우
          return 0;
        }	
        출처 : https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array/sort
    * reduce()
    	누산기(accumulator) 및 배열의 각 값(좌에서 우로)에 대해 (누산된) 한 값으로 줄도록 함수를 적용합니다.
        함수 파라미터
        	callback(이전값, 현재값, 현재 인덱스, 배열), 초기값
    * from()
    	유사 배열 혹은 반복가능한 객체로부터 새 Array 인스턴스를 만듭니다.        
        출처 : https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array/from
        
        
### String
	* includes()
        하나의 문자열이 다른 문자열에 포함되어 있는지를 결정하고,그 결과를 true 또는 false 로 반환합니다.
        대소문자를 구별
        출처 : https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/String/includes
        
### 비구조화 할당
	const [변수명1, 변수명2] = lastOne.split(', ');
    
	이와 같이 배열을 한꺼번에 다른 이름으로 변수로 받을 수 있음.
    비구조화 할당(destructuring assignment) 구문은 배열 또는 객체에서 데이터를 별개(distinct) 변수로 추출할 수 있게 하는 JavaScript 식(expression)입니다
    변수는 기본 값이 할당될 수 있습니다
    
    예시 )
    
    [a, b, ...rest] = [1, 2, 3, 4, 5];
    console.log(a); // 1
    console.log(b); // 2
    console.log(rest); // [3, 4, 5]

    ({a, b} = {a:1, b:2});
    console.log(a); // 1
    console.log(b); // 2

    ({a, b, ...rest} = {a:1, b:2, c:3, d:4});
    //ES7 - Firefox 47a01에서 구현되지 않음
    
    출처 : https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment