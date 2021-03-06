# HTML5의 이해



웹 어플리케이션 개발을 통해 SW 개발 방법 및 학습 과정을 익히기 위해서



# HTML

- Hyper Text Markup Language
- 웹용콘텐츠의 구조를 지정하는 컴퓨터언어
- 웹서버에 저장되어 클라이언트 웹부라우저의 요구에 따라 불려지는 문서
- **웹 브라우저**에 불려진 HTML은 웹 브라우저에 의해 해석되어 내용이 화면에 보여짐



## 기존 HTML의 한계

90년 월드 와이드 웹과 함께 탄생 -XHTML_업계지지를 얻지못함 - 웹 기반 사업과 기술 표현하기에 부족

- 최근 웹기반사업과 기술


1. 웹기반사업과 기술의 발전에 따른 HTML의 한계 극복

   -Ajax : JavaSscript를 이용하여 웹서버와 동기화된 웹의 한계극복

   -Web2.0

2. 동적인 웹을 위한 표준화 된기술 요구

   -게임 웹 어플리케이션을 비롯해 일반 웹 사이트들도 동적인 웹에대한 요구증가

3. WHATWG 탄생과 활동

   -탄생

   - 웹관련 업체들은 자체적으로 워킹 그룹을 만들어활동
   - 시장의 요구를 분석하고 필요한 기술을 정리

   -활동

   HTML 명세서 작업, 2008년 W3C  HTML5 초안발표, 9년 W3C XHTML2 개발 중단



HTML5의 의미 : 웹 기술 발전에 큰 전환점

- 기존 HTML의 한계

  웹 기반 사업과 기술의 발전을 못따라감

  동적인 웹을 위한 표준화 된 기술을 요구

  W3C의 XHTML2로의 발전예고

  -> WHATWG 탄생

  ​	시장 요구에 부응하지 못하는 W3C에 실망한 웹 관련 업체와 단체가 자체적으로 만든 워킹그룹

  ​	웹기술과 시자으이 요구를 분석하여 HTML5 명세서 작업착수



- 실용적 설계
  
  - 기존 기술을 바탕으로 새로운 기술추가
  - 문법강요하지 않음
  - 기존 HTML의 효율적인 요소 추가
- 안전한 보안
  
- 표현과 내용의 완벽한 분리

- 플러그 인 없이 미디어 처리 및 동적 작동

  - 자체적으로 2D, 3D 처리 가능

  - 웹 브라우저가 다양한 미디어 처리

  - 다양한 이벤트 제공

    (Java Script를 이용해야하지만)

- 최신 웹 기술 수용 
  
  - 지오로케이션, 웹소켓, 웹스토리지, 웹워커 등

## 텍스트에디터

준비

- HTML은 텍스트파일

- 단순 텍스트 파일을 생성하는 어떠한 '텍스트 에디터'에서도 작성가능

  (메모자으 워드패드, 워드프로ㅓ세서)

- 전문적인 텍스트 에디터 : 각종 컴퓨터 언어 프로그래밍에 ㅗ치적화

장점

1 컬러링

2 에러확인을 편하게 해주는 라인 넘버링

3  코드 정리를 도와주는 인덴트 기능

4 편리한 텍스트 이동

5 코드 제안과 자동 완성

6 향상된 검색과 치환 기능

7 기타 프로그래밍 관련 기능들

- 무료로 사용할수 있는 전문적인 텍스트 에디터

  Notepad++, Komodo Edit, Aptana Studio3



## Doctype 지정하기와 HTML 구조

- DOCTYPE 지정하기

  ? -  HTML은 여러 버전이 존재하므로 Doctype을 명시해야함

  - 기존 DOoctype은 매우 길고 복잠한 DTD명시해야 했다.

  - HTML5의 실용성 원칙으로 인해 짧아졌따.

    `<!DOCTYPE html>`

  - 지정이유 : 웹브라우저가 정확히 HTML을 표현하기 위해 버전명시
  - 표시방법 : HTML 문서 가장 앞에 DOCTYPE 을 표시
  - HTML5 간단하고 실용적으로 정의  <!DOCTYPE html> 이라고 치면됨

- HTML 서식 : HTML 작성 규칙

  - 요소(Element) : HTML의 마크업 명령어
    - HTML은 마크업 언어이므로 콘텐츠와 함꼐사용
    - 대소문자 구분하지 않음

  - HTML 요소의 표현

    - 콘텐츠와 HTML요소와 분리하기 위해 요소를 꺽쇠로 둘러쌈 - 태그

    - 예

      <p> 문단의미, -- 태그라 부름

- 서식 : 규칙

  - 요소의 볌위

    요소가 콘텐츠의 구조 정의

    -> 요소가 영향력을 미치는 콘텐츠의 범위 중요

  - 단독으로 사용되는 요소

    `<br> - 줄바꿈 <img> : 이미지요소`

  - 요소의 속성기술

    - 요소의 속성 : HTML요소의 필수적, 부가적인 설정 값 의미

    - 속성 기술 법:

      1. 요소명 뒤에 공백을 하나 두고 속성명 = "속성값"의 형식으로 기술

         예 : < a href="next.html">

      2. 요소의 속성이 하나 이상일 경우 : 첫 번째 속성 다음에 공백을 두고 속성명="속성값"을 연결해 기술

         예 : `<img src="img/logo.jpg" alt="Company Logo">`

      3. 속성값은 따옴표 또는 쌍따옴표 표시

         예 : `<div id='logo'> 또는 <div id="logo">`





### HEAD 설정하기

- HEAD에 위치하는요소

  1. 타이틀 지정

     : 제목

     웹브라우저 타이틀바에도 나타남

     즐겨찾기나 북마크를 저장할때도 사용됨 - 적절한 타이틀 선정

  2. 문자 인코딩

     작성위치 : head

     텍스트 에디터의 문자 인코딩 설정 : HTML 헤더부분에 설정한 문자 인코딩

  3. 메타 요소 : 메타 데이터 정의하는 부분

     3.1 메타 데이터 : 파일에 관한 정보를 가지고 있는 데이터

     3.2 HTML의 메타 요소의 필요성

     - 구글등 유명 검색 로봇에 의해 수집되는 정보 : 사이트 홍보에 유리
     - HTML 파일에 대한 정보를 기록

     3.3 메타요소 사용방법

     - 메타요소 : 마침요소가 필요없는 단독요소

       `<metaname ="keywords" contents="adsf">`

  4. 외부 파일 연결

     웹페이지는 (HTML - 콘텐츠의 구조정의 , CSS - 콘텐츠의 레이아웃과 표현등 외향을 정의 JS - 콘텐츠의 작동을 정의 )로 이루어짐

     다른 파일로 분리하는것이 유지보수에 유리

     - 외부 CSS 파일 연결

       `<link rel="stylesheet" href="CSS/style.CSS">`

     - 외부 자바스크립트 파일 연결

       `script src="js/script.js"></script>`

  #### Q. HTML5에서 기존 HTML과 달라진 meta 요소와 Empty요소에 대하여 작성

  `meta 요소는 지금까지의 HTML요소와 다르게 시작요소만을 가지고 맺음 요소는 존재하지 않습니다. 기존 HTML 요소가 웹브라우저에 해당 콘텐츠ㅏ 어떤 구조와 의미를 갖는지 알려주는 역할을 했다면 meta요소는 웹 브라우저에게 문서 정보를 알려주는 역할을 합니다. 그렇다보니 일반적인 HTML 요소가 내용을 감싸는 형식이라면 meta 요소는 속성과 속성 값의 정보를 담고 있을 뿐 내용을 감싸는 것은 아닙니다. 그래서 내용을 가지고 있지 않은 요소 즉 Empty요소라고 부릅니다. 이러한 Empty 요소에는 img, area, br, hr, input 등이 있습니다.`

  #### Q. HTML 파일에서 외부 CSS 파일을 연결하는 방법은?

  `<link rel="stylesheet" href="파일경로">`

  #### Q. 웹에 동적인 작동을 추가할 수 있는 플래쉬에 대한 설명

  `플래쉬는 폐쇄적이고 독점적 이여 개발사의 이익에 좌지우지 된다.`





### 정리(시험대비)

- 웹표준과 브라우저전쟁

- 현재의 웹표준

  W3C에서 만들고 있었고(연구원 위주)

  WHATWG 에서도 만들고 있었따(기업위주(apple, google, 마소 등등))

  싸웠다

  대 - 통합 (두단체가 같이 협업을해서 웹플랫폼을 만들고 정의 해나가기로함)

- can i use (html,css 등을 특정 브라우저에서 쓸 수 있는가?)

  #### HTML(Hyper Text Markup Language)

  - why?

    hyper text - 다른문서에 연결되는 링크를 지니고 있는 것 (http - hyper text transfer protocol)

    markup - 그냥 있는 문서들을 잘 볼수 있도록 문서의 구조를 잡는 것

  - 기본 구조

    DOM(document object model) 트리

    - 요소(element) - 태그

    - 속성(Attribute)

    - head

      문서제모그 문자 인코딩 등의 문서정보

      메타데이터를 통해 웹문서에 대한 추가정보선언

      - 메타 데이터를 표현하는 새로운 규약, open graph protocol
      - HTML 문서의 메타 데이터를 통해 문서의 정보를 전달
      - 페이스북에서 만들었으며, 메타정보에 해당하는 제목, 설명등을 쓸수 있도록 정의

    - 시맨틱 태그

      HTML5에서 의미론적요소를 담은 태그의 등장, div

- HTML 구조화(상)
  - 인라인 / 블록요소(CSS에서 자세한 내용을 다룹니다.)
  - 그룹 컨텐츠
  - 텍스트 관련 요소

- (하)

  - form

    서버에서 처맅될 대이터~

  - table
  - 