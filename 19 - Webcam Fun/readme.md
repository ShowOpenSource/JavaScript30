#Video Source 분석

## 목적

Video 소스 코드를 분석하고 어떤 메서드가 있는지 알아봄

## 새로운 개념 및 이벤트

### Navigator

window.navigator 객체는 방문자의 브라우져 정보들을 포함하고 있다.

참고 : http://www.w3schools.com/jsref/obj_navigator.asp

window.navigator.MediaDevices

MediaDevices 인터페이스는 카메라나 마이크 같은 인풋 미디어 디바이스와 연결하게 해준다.

참고 : https://developer.mozilla.org/ko/docs/Web/API/MediaDevices

### window.URL.createObjectURL

특정 파일 객체나 로컬 파일 또는 데이터의 참조를 가리키는 새로운 객체 URL을 생성한다.
생성한 값은 현재 창이나, 객체를 생성한 문서 내에서만 유효하다.
새 객체 URL은 특정 FILE 객체나 BLOB 객체로 표현 할 수 있다.

```
 var objectURL = window.URL.createObjectURL(blob);
```

매개변수로 전달한 blob는 URL을 생성할 File 객체나 Blob 객체이다.
생서된 objectURL은 해당 파일의 전체 내용을 URL 텍스트로 변환한 값이다.

객체의 URL의 사용을 마쳤다면, 아래 메서드를 호출해 메모리에서 해제해주는 것이 좋다.

```
    window.URL.revokeObjectURL(objectURL);
```

참고 
	- https://developer.mozilla.org/en-US/docs/Web/API/URL/createObjectURL
	- http://ohgyun.com/446

### Canvas

ctx.getImageData()

해당 메서드를 사용하면 canvas context에서 각각 픽셀의 데이터를 가져올수 있다.

### document.createElement

지정된 태그 이름ㅇ르 가지는 엘리먼트를 생성한다.

참고 : https://developer.mozilla.org/ko/docs/Web/API/Document/createElement

### insertBefore

해당 엘리먼트 삽입 전에 해당 엘리먼트를 대입한다. 

```

var newItem = document.createElement("LI");       // Create a <li> node
var textnode = document.createTextNode("Water");  // Create a text node
newItem.appendChild(textnode);                    // Append the text to <li>

var list = document.getElementById("myList");    // Get the <ul> element to insert a new node
list.insertBefore(newItem, list.childNodes[0]);  // Insert <li> before the first child of <ul>

```
참고 : http://www.w3schools.com/jsref/met_node_insertbefore.asp