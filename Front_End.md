
Front-End
https://github.com/kamranahmedse/developer-roadmap
https://raw.githubusercontent.com/kamranahmedse/developer-roadmap/master/img/frontend.png
2017버전 : https://t1.daumcdn.net/cfile/tistory/2560A33B58FE281731

1. 주요 용어 
1-1) Platform : 어플리케이션을 작동시키기 위한 "기반 OS"나 "기술환경"
      1. 하드웨어 플랫폼
      2. 소프트웨어 플랫폼 : 여러가지 기능들을 제공해주는 공통 실행환경 ( 브라우저, JAVA ...)
      3. 서비스 플랫폼 (SNS)

1-2) Framework : 특정 프로그램을 개발하기 위한 여러 요소들과 메뉴얼인 룰을 제공하는 프로그램
               : AngularJS, Vue, Spring, Django, Ruby on Rails, Bootstrap

1-3) library : 개발 도구의 모음입니다.

1-4) Moudle Bundling : 웹 애플리케이션을 구성하는 몇십, 몇백개의 자원들을 하나의 파일로 병합 및 압축 해주는 동작
모듈 : 웹 애플리케이션을 제작에 필요한 HTML, CSS, Javascript, Images, Font 등 이 파일 하나하나가 모두 모듈
번들러 : 소프트웨어 및 일부 하드웨어와 함께 작동하는데 필요한 모든 것을 포함하는 패키지

1-6) Pre-Processor(전처리기)
컴파일러가 소스 파일을 컴파일하기 전에 먼저 수행되는 프로그램(처리기)

1-7) TDD(Test Driven Development) : 테스트 주도 개발

1-8) 하드웨어 생산자는 퍼스트 파티(first party)로, 소프트웨어 개발자는 서드 파티(third party)

1-9) 정적, 동적
정적은 컴파일 시점, 동적은 런타임 시점에 타입이 체크되어진다.



1-11) Node.js
Node.js는 웹브라우저에 종속적인 자바스크립트를 ( Chrome V8 엔진을 제공하여) 브라우저 외의 다른 환경에서도 사용할 수 있게 해주는 소프트웨어 플랫폼 (런타임?) 입니다.
http서버가 내장되어 있기 때문에 보통은 서버로 많이 사용합니다.




2. Package Managers(패키지 매니저) 
: 패키지를 다루는 작업을 편리하고 안전하게 수행하기 위해 사용되는 툴이다.
: 여기서 패키지를 다루는 작업이란 패키지를 설치, 업데이트, 수정, 삭제하는 작업을 의미한다.

2-1) npm : node package manager
Node.js에서는 자주 쓰이고 재사용되는 자바스크립트 코드들을 패키지로 만들어서 사용 가능.
이런 패키지를 모아놓은 저장소가 npm.
Node.js를 설치하면 자동으로 npm이 설치.
package.json : 패키지명과 함께 패키지 버전도 관리

[주요 명령어]
npm install : npm 설치
npm -v : 버전 체크
npm update -g npm : 최신 버전 업데이트
npm init : package.json 생성
const 변수이름 = require(패키지이름) : 패키지 사용

2-2) yarn : 자바스크립트의 새로운 패키지 매니저
페이스북, Exponent, 구글과 Tilde의 엔지니어 그룹들이 함께 협력하여 npm의 핵심 이슈를 해결하기 위해 만든 패키지 매니저.
이 새로운 자바스크립트 패키지 매니저가 얀(Yarn)이다. 보다 빠르고 안정적이며 보안성이 뛰어나다고 주장하고 있다.


3. CSS
2-1) CSS Architecture 
- BEM (Block Element Modifier)
- OOCSS(Object Oriented CSS)
- SMACSS (Scalable Modular Architecture CSS)

2-2) CSS Preprocessor 
	sass(언어), postcss(자바스크립트 기반의 플러그인을 사용하여 CSS 기능을 자동화하는 소프트웨어 개발 도구), less(언어), stylus 
2-3) at-rule (@규칙)
- @charset
- @import
- @media
- @page
- @font-face
- @namespac



3. JavaScript
https://t1.daumcdn.net/cfile/tistory/9997C73359B2B4011C

3-1) 클래스 > 객체 > 인스턴스
클래스는 틀(설계도)이고 : 연관 변수(필드)와 메소드로 구성
객체는 추상적 대상 선언(설계도로 지은 집) : 속성과 메소드로 구성
인스턴스는 구체적 실체화(설계도로 지은 내집)라고 보면 된다 : 메모리에 할당된 객체 , 생성된 복제본을 의미
* 클래스로부터 객체를 선언하는 과정을 클래스의 인스턴스 화


* 스택 : 후입선출 자료 구조  
* 스코프 : 함수 범위
* 메소스 : 객체와 관련된 함수
* lexical scope : 접근 가능한 범위
* 클로저 : 함수 안에서 선언된 내부함수(익명함수)로 접근 범위는 lexical scope

* 이벤트 루프 : 호출 스택이 비워지면 태스크 큐에서 함수를 하나씩 호출 스택으로 밀어 올립니다.
* 이벤트 버블링 : 자식의 이벤트가 부모에도 전달되는 것
* 이벤트 드리븐(이벤트 기반) : 이벤트가 발생할 때 미리 지정해 둔 작업을 수행하는 것 (일련의 동작을 정의하고 등록된 상태가 이벤트 리스너에 등록된 상태)

* Synchronous (작업 순서 보장) VS Asynchronous (작업 순서 비보장) : 구분 기준은 작업 순서
* Blocking(작업의 멈춤, 대기(Wait)) VS Non-Blocking(대기(Wait) 없음) : 구분 기준은 통지(제어권)
  - Blocking : 작업을 시작하고 작업이 끝날때까지 대기하다가 즉석에서 완료 통지를 받는다.(작업이 멈추는 동안 다른작업이 끼어들수 있는지 없는지는 다른 얘기)
  - Non-Blocking : 대기 없이 완료시킨 후 나중에 통지받는 개념 (작업의 시작 이후 완료시까지 대기하지 않고, 완료시킨다.)

[ locking-NonBlocking-Synchronous-Asynchronous ]
Sync-Blocking : 작업순서는 보장. 호출에서 반환까지 대기
Sync-NonBlocking : 작업순서 보장. 호출(콜백)에서 반환까지 대기 없이 완료.
Async-Blocking : 작업순서도 비보장. 호출에서 반환까지 대기 
Async-NonBlocking : 작업순서 비보장. 호출(콜백)에서 반환까지 대기 없이 완료.  
https://jins-dev.tistory.com/entry/%EB%8F%99%EA%B8%B0Synchronous-%EC%9E%91%EC%97%85%EA%B3%BC-%EB%B9%84%EB%8F%99%EA%B8%B0Asynchronous-%EC%9E%91%EC%97%85-%EA%B7%B8%EB%A6%AC%EA%B3%A0-%EB%B8%94%EB%9D%BDBlocking-%EA%B3%BC-%EB%84%8C%EB%B8%94%EB%9D%BDNonBlocking-%EC%9D%98-%EA%B0%9C%EB%85%90
https://heecheolman.tistory.com/48
http://homoefficio.github.io/2017/02/19/Blocking-NonBlocking-Synchronous-Asynchronous/
* setTimeout 0도 기본적으로 4ms의 지연 시간을 노드는 1ms의 지연 시간을 갖고 있습니다.


3-2) OOP(객체지향프로그래밍)의 형태
1. 캡슐화 (Encapsulation)
2. 상속 (Inheritance)
3. 다형성 (Polymorphism)
4. 추상화 (Abstraction)

클래스(일반 언어  C++, JAVA) 기반 VS 프로토타입 (자바스크립트) 기반
* 차이점 : 클래스와 인스턴스
* 클래스 -> 클래스는 틀이고, 인스턴스는 클래스가 실체화된 것
      -> 즉, 클래스는 클래스로부터 상속되고 하위클래스와의 관계가 만들어진다. (계층구조)
* 프로토타입 -> 프로토타입은 클래스와 인스턴스의 차이를 두지 않는다.
          -> 실체화된 객체로써, 객체는 다른 객체로부터 상속된다.


3-3) Node.JS 






1) Webpack : 모듈 번들러(Module Bundler)입니다.


2) Babel

3) ESLint








Vue.js

Vue


npm


* Node.JS 내장 모듈은 검색해서 사용



* Runtime 런타임 : 어떤 프로그램이 실행되는 동안의 Time
* Compile tiem 컴파일타임 : 고급 언어(프로그래밍 언어)를 기계어로 변경하는 과정



[JS Enjine]
<img src="https://miro.medium.com/max/2048/1*4lHHyfEhVB0LnQ3HlhSs8g.png">

* UI (User Interface) : 사용자와 사용자가 다룰 대상(하드웨어 혹은 소프트웨어)을 연결 하는 매개체

* API(Application Programming Interface, 응용 프로그램 프로그래밍 인터페이스)
  : 응용 프로그램에서 사용할 수 있도록, 운영 체제나 프로그래밍 언어가 제공하는 기능을 제어할 수 있게 만든 인터페이스 
  : 프로그램과 프로그램을 연결해주는 매개체

* Web API : 자바스크립트 엔진이 아닌 브라우저에서 제공하는 API (DOM, Ajax, Timeout, requestAnimationFrame, Promise 등)


* Stack(스택) : 자료구조 중 하나, 후입선출(LIFO, Last In First Out)의 룰을 따른다.

* Queue(큐) : 자료 구조 중 하나, 선입선출(FIFO, Frist In Frist OUT)의 룰을 따른다.
[ Callback Queue 순서 ] 
Microtask Queue(Job Queue) : Promise의 then() 의 콜백
Animation Frames : requestAnimationFrame
Task Queue(Event Queue) : setTimeout 콜백

Event Loop는 Call Stack과 Callback Queue의 상태를 체크하여,
Call Stack이 빈 상태가 되면, Callback Queue의 첫번째 콜백을 Call Stack으로 밀어넣는다.
이러한 반복적인 행동을 틱(tick) 이라 부른다.


* MongoDB 자바스크립트로 된 데이터베이스
* LESS 자바스크립트로 된 CSS


* LTS 여러 버전이 동시에 지원되면서 순차적으로 종료해나가는 시스템





### Browser의 렌더링 과정

## 렌더링
사용자의 요청이 오면 서버로부터 HTML 파일을 받아 브라우저에 뿌려주는 과정

## 렌더링 엔진
렌더링 엔진의 역할은 요청 받은 내용을 브라우저 화면에 표시하는 일을 담당

|브라우저    | 렌더링 엔진                   |
|-----------|------------------------------|
|IE         | `Trident`                    |
|Edge       | `EdgeHTML, Blink`            |
|Chrome     | `Webkit, Blink(버전 28 이후)` |
|Safari     | `Webkit`                     |
|FireFox    | `Gecko`                      |

* 크롬 브라우저(정확히는 크로미움은)는 사파리 브라우저에서 사용하는 Webkit을 사용하다가 버전 28 이후 Webkit 소스를 Fork 하여 Blink 엔진을 만들어 사용하고 있습니다.


## 렌더링 엔진 동작 과정
![렌더링 엔진 동작 과정](https://beomy.github.io/assets/img/posts/browser/webkit_rendering_engine_process.png)  
렌더링 엔진 동작 과정(원본 출처: "<a  href="https://beomy.github.io/tech/browser/browser-rendering/">동작 과정 상세</a>
1. HTML을 파싱하여 DOM 노드를 만듭니다. 이 DOM 노드들을 병합하여 DOM 트리를 만듭니다.
2. CSS를 파싱하여, 스타일 규칙을 만듭니다.
3. DOM 트리와 스타일 규칙을 사용하여, Attachment라는 과정을 통해 Render 트리를 생성합니다.
4. Render 트리를 배치(Layout)합니다.
5. Render 트리를 화면에 그림(Painting)니다.

# 1. 객체 모델 생성
1-1) HTML을 파싱하여 DOM(Documnet Object Model) 노드 생성 : DOM 트리 (HTML 구조 표현)
1-2) CSS를 파싱하여 CSSOM(CSS Object Model) 생성 => CSSOM 트리 (스타일 규칙) 

# 2. 렌더 트리 (Render Tree) 생성
독립적인 DOM 트리와 CSSOM 트리를 결합(어태치먼트Attatchment) 하여 렌더링 트리를 형성

# 3. 레아이웃 (리플로우)
렌더 트리는 DOM 트리와 CSSOM 트리에 의해 정의된 스타일만 계산하기 떄문에
브라우저에 출력하기 전 기기의 뷰포트 내 각 노드의 정확한 크기와 위치를 계산 한다.

# 4. 페이팅, 래스터라이징 (리페인팅)
렌더링 엔진은 페인트 이벤트를 발생시켜 렌더링 트리를 화면에 그린다.
페인트 단계에서는 위치나 크기를 제외한 나머지 색상이나 투명도 같은 CSS 속성들을 실제 픽셀로 변환 한다.

# 5. 합성 & 렌더 (Composite & Render)
모든 객체들을 조합하여 실제 브라우저 화면을 업데이트한다.

# 6. 리플로우, 리페인팅
렌더링이 완료된 상태에서 사용자의 인터랙션에 의해 화면의 일부 영역이 변경되면 `리플로우` , `리페인트`  발생
- 레이아웃이 변경될 경우 `리플로우` , `리페인트` 
- 레이아웃에는 영향을 주지 않지만 가시성에는 영향을 주는 엘리먼트가 변경될 때는 `리페인트` 
* 레이아웃 변경
<ul>
  <li>DOM 엘리먼트 추가, 제거 또는 변경</li>
  <li>CSS 스타일 추가, 제거 또는 변경</li>
  <li>CSS 스타일을 직접 변경하거나, 클래스를 추가함으로써 레이아웃이 변경될 수 있다. 엘리먼트의 길이를 변경하면, DOM 트리에 있는 다른 노드에 영향을 줄 수 있다.</li>
  <li>CSS3 애니메이션과 트랜지션. 애니메이션의 모든 프레임에서 리플로우가 발생한다.</li>
  <li>offsetWidth 와 offsetHeight 의 사용. offsetWidth 와 offsetHeight 속성을 읽으면, 초기 리플로우가 트리거되어 수치가 계산된다.</li>
  <li>유저 행동. 유저 인터랙션으로 발생하는 hover 효과, 필트에 텍스트 입력, 창 크기 조정, 글꼴 크기 변경, 스타일시트 또는 글꼴 전환등을 활성화하여 리플로우를 트리거할 수 있다.</li>
</ul>
* 가시성 변경
opacity, background-color 등


## 참고
https://memory.today/dev/36
https://beomy.github.io/tech/browser/browser-rendering/
https://yceffort.kr/2019/08/12/how-browser-work/
https://velog.io/@ru_bryunak/%EB%A0%8C%EB%8D%94%EB%A7%81%EC%9D%B4%EB%9E%80