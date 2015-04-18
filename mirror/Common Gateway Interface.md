사용자가 웹 서버에서 정보를 찾거나 기록하는 행위를 가능하도록 해 주는 기술의 명칭이다. 본래 처음 웹이 개발될 때 채택된
[HTML](HTML.md)은 서버에 있는 문서를 단순히 보여주는 것 뿐이었다. 이 때문에 거꾸로 사용자가 서버에 정보를 기록하거나
직접 정보를 찾거나 하는 일은 불가능했다. CGI는 이 HTML의 약점을 보완하기 위해 나온 기술로, HTML에서 불가능한 정보 찾기 밎
기록을 가능하게 해 주는 역할을 한다.

웹 서버에서 CGI는 다음과 같이 동작한다.

  1. HTML에서 폼(Form)을 통해 요청할 정보를 보낸다.  
(이 때문에 HTML에는 input, textarea, option 같은 폼 태그들이 있다. 이들 폼 태그를 입력하면 웹 브라우저 상에서
프로그램에서나 볼 법한 입력창, 체크박스, 라디오 버튼 등이 구현되는 것을 볼 수 있다.)

  2. CGI에서는 폼에서 지정한 서버 프로그램으로 정보를 전달한다.
  3. 서버 프로그램에서는 전달된 정보를 해석하여 그에 맞게 프로그램을 수행한다.   

이 때문에 CGI를 통해 웹 서버에 정보를 찾거나 기록하는 서버 프로그램이 필수적으로 필요하다. 초창기에는
[C언어](C%EC%96%B8%EC%96%B4.md) 같은 컴파일러 언어를 이용해서 직접 CGI와 통신하는 서버 프로그램을 만들어
썼으나, 유지보수가 너무 불편하다는 단점이 있었다. 이 때문에 인터프리터 방식으로 동작하는 [스크립트언어](%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8%20%EC%96%B8%EC%96%B4.md) 규격을 만들고,
이 스크립트 언어를 구동시키는 서버 프로그램을 컴파일러 언어로 만들어 실행시키는 방식을 쓰게 되었다. 오늘날 많이 쓰이는
[Python](Python.md), [Perl](Perl.md), [PHP](PHP.md),
[JSP](JSP.md), [ASP](ASP.md) 등등이 대표적인 서버 사이드 스크립트 언어들로, 이들 언어를 쓰려고 하면 먼저
웹 서버에 모듈 소프트웨어를 설치해야 하는 이유는 이 때문이다. CGI를 통해 온 정보가 먼저 모듈 소프트웨어로 들어간 뒤, 최종적으로 서버
스크립트 소스코드를 돌려서 실행시키기 때문이다.

오늘날 웹 서버 소프트웨어 중 이걸 지원하지 않는 프로그램은 **없다**. 웹 서버에서 핵심적인 기능이나 마찬가지이기 때문에, 이게 없으면
**검색**부터 안 된다. CGI를 지원하는 프로그램의 경우 웹 서버 [OS](OS.md) 위에서 돌아가는 프로그램이다 보니 웹 서버에
설치된 OS에서 실행되도록 만들어져야 한다. 위의 모듈 소프트웨어들이 모두
[리눅스](%EB%A6%AC%EB%88%85%EC%8A%A4.md)와
[윈도우](%EC%9C%88%EB%8F%84%EC%9A%B0.md)용이 따로 나오는 것도 이 때문이다.
