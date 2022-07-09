## HTML

- HTML 기능
- HTML의 기본 문법
- HTML의 부모태그와 자식태그
- HTML 다양한 태그의 활용
- VS Code 코드를 보기좋게 만드는 Prettier 설치하기
- Ghost Rain 화면 구성하기

---

### !DOCTYPE

> 참고 : https://www.w3schools.com/tags/tag_doctype.asp

- 브라우저에게 전달되는 문서의 정보를 알려주기 위한 용도
- HTML 태그가 아님
- Chrome, Edge, Firefox, Safari, Opera 브라우저에서 지원
- HTML5 이전에는 DTD(Document Type Definition)를 정의해야했기에 복잡했으나, HTML5 부터는 간단하게 정의 가능

### title

> 참고 : https://www.w3schools.com/tags/tag_title.asp

- 문서의 제목을 의미
- 브라우저 상단 바 이름 지정
- 검색 엔진(SEO)에서 중요한 역할을 수행 (검색 결과)
- 가능하다면 50-60을 초과하지 않는 긴 제목을 작성하는 편이 좋음 (단어만 나열한 내용은 비추천)
- Chrome, Edge, Firefox, Safari, Opera 브라우저에서 지원

### charset, lang

> 참고 : https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta#attr-charset

- HTML 문서의 문자 인코딩 방식을 명시
- HTML5 이전에는 `http-equiv` 속성을 이용하여 인코딩 방식을 명시해왔지만, HTML5 부터는 간단하게 정의 가능
- Chrome, Safari, Opera 브라우저에서 지원 (Edge는 12, Firefox는 1)

### ASCII Code

ASCII Code는 American Standard Code for Information Interchage의 약자로 문자에 대해 각각 번호를 지정하여 관리하고 있는 집합체이며 가장 기초가 되는 문자 코드다. 프로그램이나 다른 컴퓨터와 통신할 때 문자와 기호가 숫자로 변환될 필요가 있어 ASCII Code가 개발되었다. ASCII Code에서는 7비트 부호로 128개의 숫자가 알파벳, 숫자, 특수문자, 제어문자가 할당되어있다.

ASCII Code는 한 문자당 1바이트로 이루어져있데 왜 7비트로 표현될까?

나머지 1비트는 Parity 비트로 데이터의 에러를 감지하기 위해 사용한다. 7 자리의 이진수에서 1의 개수가 홀수이면 끝에 1을 붙이고 1의 개수가 짝수이면 끝에 0을 붙인다. 따라서 ASCII Code는 총 7자리의 이진수를 문자로 나타낼 수 있어 2의 7승 - 128개의 문자로 표현할 수 있다는 것이다.

### Unicode

Unicode는 ASCII Code와 같이 집합체의 한 종류로, 전 세계의 모든 문자를 컴퓨터에서 일관되게 표현하고 다룰 수 있도록 설계된 산업 표준이다. 전 세계의 모든 문자를 담는 ISO/IEC 10646 코드표를 사용하여 각 언어와 문자 체계에 따른 충돌 문제를 해결했다. 즉, 유니코드를 사용하면 통일된 환경에서 문자를 깨뜨리지 않고 사용할 수 있다. OS, 프로그램, 언어와 상관없이 문자마다 고유한 코드값을 제공하고 있으며, 16비트 - 즉, 최대 65,536자 까지 표현할 수 있다.

왜 2바이트를 사용할까?

ASCII Code의 경우에는 영어만을 고려하여 개발되었기 때문에 1바이트로 표현이 가능했지만, Unicode는 다른 언어권의 문자를 정의하기 위해 2바이트를 사용한다. 따라서 2의 16승으로 65,536개의 문자로 표현할 수 있다.

### UTF-8

UTF-8은 Unicode를 위한 가변 길이 문자 인코딩 방식 중 하나다. Unicode Transform Format - 8bit 의 약자이며, 1바이트를 **기준**으로 인코딩한다는 의미다. 예를 들어 'a'는 1바이트이며 '가'는 2바이트를 가진다. 그리고 각 가변을 구분하기 위해 표식을 넣게 되는데, 2바이트는 110으로 시작하고 3바이트는 1110으로 시작한다. 그 외 나머지 바이트는 10으로 시작되는데, 이는 일종의 약속이라고 한다.

근데 왜 Unicode가 있는데 UTF-8 인코딩 방식이 나온걸까?

가장 첫 문장에서 UTF-8은 가변 길이 문자 인코딩 방식이라고 했는데 바로 이 점이 질문의 답이다. Unicode는 영어만을 표현하는 ASCII Code와는 다르게 다른 언어권의 문자까지도 고려했지만, 영어를 표현할 때 1바이트 한글은 2바이트 특수문자는 3바이트로 - 즉, 가변적인 문자의 길이로 표현되기 때문에 문제가 발생했기 때문이다. 따라서 컴퓨터에게 혼란을 주지 않기 위해 어떤 글자는 1바이트로, 어떤 글자는 2바이트로 읽을지 정해줘야했는데, 이를 명시하는 방법이 바로 인코딩 방식이다. 인코딩 방식은 정말 다양하며, 각 인코딩 방식마다 컴퓨터가 어떤 글자를 만났을 때 얼만큼씩 읽어줘야하는지 미리 알려주는 역할을 수행한다.

UTF-8에 대해서 다시 정리해보자. UTF-8은 Unicode 한 문자를 나타내기 위해서 1바이트에서 4바이트까지 사용하고 이를 가변 길이 인코딩 방식이라고 한다. ASCII Code의 문자들은 1바이트로 하나의 문자를 표현할 수 있는데, 모든 문자를 4바이트로 표현하게 되면 지나친 저장소의 낭비가 되므로 ASCII Code로 표현 가능한 것은 1바이트, 그 이외의 문자는 2바이트 이상을 사용하도록 정의된 것이 바로 UTF-8이다. 앞에서 설명했 듯이 가변 길이를 판단하는 기준은 가장 첫 번째 비트가 어떤 것인지 확인해보면 된다.

- 0xxxxxxx : 첫번째 바이트가 0으로 시작하면 0이외의 7비트를 아스키로 인식한다.
- 110xxxxx 10xxxxxx : 두번째 바이트까지 읽어서 하나의 문자로 표현
- 1110xxxx 10xxxxxx 10xxxxxx : 세번째 바이트까지 읽어서 하나의 문자로 읽어서 하나의 문자로 표현
- 111110xxx 10xxxxxx 10xxxxxx : 네번째 바이트까지 읽어서 하나의 문자로 표현

### Character Set Summary

나만의 방식으로 정리하자면 다음과 같다.

- ASCII Code는 영어만을 표현하는 문자 코드 (128개)
- Unicode는 영어뿐만 아니라 다른나라 언어권까지 표현하는 문자 코드 (65,536개)
- UTF-8은 Unicode의 인코딩 방식 중 하나로, 1바이트에서 4바이트까지 각 문자마다 가지는 바이트 크기를 가변적으로 표현이 가능

### head (meta)

> 참고 : https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta

head 태그에는 `<title>, <style>, <meta>, <link>, <script>` 요소들의 부모 태그다. 그 중 부가적인 정보를 제공해주는 meta 태그에 대해서 정리해보자.

메타 태그에 사용 가능한 속성은 `charset, content, http-equiv, name` 총 4개다. `charset`을 제외한 나머지 속성을 살펴보자.

먼저 `content`는 사용되는 속성에 따라 `http-equiv` 또는 `name`에 대한 값이 포함된다. 쉽게 말하자면 `http-equiv, name` 속성에 들어가는 값에 대한 값을 설정할 때 사용하는 속성이라고 보면 된다.

`http-equiv`는 HTTP 헤더에 정보나 값을 제공하는 속성이다. 주로 HTML 문서에서 사용할 문서의 종류나 새로 고침등에 사용된다.

```html
<!-- content-type : 인코딩 방식 명시 (HTML5 에서는 간단하게 표현 가능) -->
<meta http-equiv="content-type" content="text/html; charset=UTF-8" />

<!-- default-type : 우선 적용할 스타일시트 명시 (단, `content` 속성값은 문서 링크의 title 속성값이나 style의 title 속성값과 일치해야한다.) -->
<meta http-equiv="default-type" content="prefereed stylesheet" />

<!-- refresh : 문서 새로고침 시간 간격 명시 -->
<meta http-equiv="refresh" content="30; url=이동할 주소" />

<!-- x-ua-compatible : 브라우저 호환성 모드 조정. `content`에 정의된 값에 따라 브라우저는 해당 버전으로 호환성 보기로 열림 (대부분 생략하는 경우가 많은 듯) -->
<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
```

`name`은 말 그대로 문서의 이름을 짓는거라고 생각하는 편이 이해하기 쉽다. 다음과 같은 목록들을 구성할 설정할 수 있다.

- author : 문서 작성자
- description : 문서에 대한 간략한 설명
- generator : 페이지를 생성한 소프트웨어의 식별자
- keywords : 쉽표로 구분된 페이지 컨텐츠와 관련된 단어들
- referrer : 문서에서 보낸 요청의 HTTP 헤더를 제어
- viewport : 뷰포트의 초기 크기에 대한 힌트를 제공
- theme-color
- color-scheme

`referrer` 속성값에 대해 `content` 값도 여러 가지가 존재한다. 내가 이해한 바가 맞다면 출처에 대한 처리를 하기 위해 정의하는 것이다.

- no-referrer
- origin
- no-referrer-when-downgrade
- origin-when-cross-origin
- same-origin
- strict-origin
- strict-origin-when-cross-origin
- unsafe-URL

그 외에도 `name` 속성에 설정 가능한 creator, googlebot, publisher, robots값들이 있는데 해당 내용은 천천히 개발하면서 알아보자.

---

### Ghost Game

**기획 초안 :**

![](/images/ghost_game_draft.png)

- 제목
- 설명
- 목숨 3개
- 플레이 타임 및 점수
- 메인 이미지
- 시작 버튼
- 플레이타임 + 점수 랭킹

**HTML 구조 잡기 :**

![](/images/ghost_game_html.png)
