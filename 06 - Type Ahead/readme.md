#Native Fetch Source 분석

## 목적

Fetch 사용법을 익힌다.

## 새로운 개념 및 이벤트

### Fetch API
	* Ajax 요청을 위해 jQuery의 $.ajax와 같은 역할을 함
	* HTTP 프로토콜의 모든 개념을 JS 에 똑같이 도입
	* Promise를 반환하여 then을 이용하여 채이닝으로 사용하면 됨. 
	* Fetch API 는 3개의 인터페이스를 도입함. 
		* Headers
		* Request
			Request 인터페이스는 HTTP 를 통해 자원을 가져오기 위해 전달하는 요청(request)
		* Response 
			fetch() 를 호출하면 그 결과로 Response 인스턴스가 반환
	* body 에 포함된 함수
		* arrayBuffer()
		* blob()
		* json()
		* text()
		* formData()

참고 : http://hacks.mozilla.or.kr/2015/05/this-api-is-so-fetching/

### RegExp 정규표현식

#### 정규 표현식을 만드는 방법 2가지
	* var re = /ab+c/;
	* var re = new RegExp("ab+c");

#### 정규 표현식 함수
	* exec
		일치하는 문자열을 찾는 메서드
		배열 반환
	* test
		일치하는 문자열을 검사하는 메서드 
		true or false 반환
	* match
		일치하는 문자열을 찾는 String 메서드
		정보를 가지고 있는 배열을 반환하거나 일치하지 않는 부분을 null로 반환  
	* search
		일치하는 문자열을 검사하는 String 메서드
		일치하는 인덱스 반환하거나 검색에 실패시 -1 반환 
	* replace
		일치하는 문자열을 찾는 String 메서드
		문자열을 대체해서 반환 
	* splite
		일치하는 문자열을 찾는 String 메서드
		해당 정규표현식을 기준으로 잘라서 배열로 반환 

출처 : https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/%EC%A0%95%EA%B7%9C%EC%8B%9D