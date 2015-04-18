  * [동음이의어](%EB%8F%99%EC%9D%8C%EC%9D%B4%EC%9D%98%EC%96%B4.md). 다른 종류의 자바는 [자바](%EC%9E%90%EB%B0%94.md) 항목 참고
  * [프로그래밍 언어](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4.md)  

![http://upload.wikimedia.org/wikipedia/commons/thumb/a/a4/Java_logo_and_wordm
ark.svg/262px-Java_logo_and_wordmark.svg.png?width=200&align=right](http://upl
oad.wikimedia.org/wikipedia/commons/thumb/a/a4/Java_logo_and_wordmark.svg
/262px-Java_logo_and_wordmark.svg.png)

[[PNG external image]](http://upload.wikimedia.org/wikipedia/commons/thumb/a/a
4/Java_logo_and_wordmark.svg/262px-Java_logo_and_wordmark.svg.png)

  

## Contents

    

1. 개요 
2. 어원 
3. C, C++와의 비교 
4. 특징 
    

4.1. 장점

    

4.1.1. 비교적 높은 생산성

4.1.2. 기기 호환성

4.1.3. 안정성

4.2. 단점

    

4.2.1. 속도 문제

4.2.2. 불편한 예외 처리

4.2.3. 표준 입출력 지원 미비

4.2.4. 언어적 불편함

    

4.2.4.1. 연산자 재정의 미지원

4.2.4.2. 명사형 생각을 강제

4.2.4.3. [클로저](%ED%81%B4%EB%A1%9C%EC%A0%80.md) 미지원

4.3. 기타

5. 변종 및 개발환경 
    

5.1. 개발환경

5.2. 다른 언어 같은 출력물

5.3. 자바로 구현한 다른 언어

5.4. 유사품에 주의합시다

6. 여담 

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=1)]

## 1. 개요 ¶

[선마이크로시스템즈](%EC%84%A0%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%8B%9C%EC%8A%A4%ED%85%9C%EC%A6%88.md)에서 1995년에 개발 `[1]`한 [객체 지향](OOP.md) [프로그래밍언어](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4.md).
2010년에 선이 [오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md)에 인수되어서 현재 저작권자는
[오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md)이다.  
<del>초딩들에게는
[마인크래프트](%EB%A7%88%EC%9D%B8%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8.md)를 돌릴수 있는
프로그램이라 카더라</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=2)]

## 2. 어원 ¶

<del>자바를 자바볼까</del> <del>[자바](%EC%9E%90%EB%B0%94#s-1.md)에서
한번[자바](%EC%88%98%EB%A9%B4.md).</del>  
[#](http://www.javaworld.com/community/node/6242)  
처음엔 고슬링 사무실 앞에 있는 나무인 OAK로 지었다가 그대로 등록하기엔 상표권에 문제가 생겨서 컨설턴트가 극단적인 방법을 도입, 오후에
개발진들을 회의실에 가둬<del>모인게 아니라</del> 마라톤 회의를 시켰고, "기분이 어떤가요" (Excited!) "무엇이 당신 기분을
좋게 만드나요?" (JAVA!)같은 연상적인 작용을 거쳐 여러가지 이름을 정하고, 그 중에서 선택했다. JAVA는 랭킹 중 네번째. 리스트의
첫번째 이름은 Silk였고 고슬링이 가장 좋아했던 이름은 Lyrics, 세번째에 올라왔던 이름이라고... `[2]``[3]``[4]` 그런데
막 지은 것 치고는 나중에 Sun사의 주식시장 등록 이름이 JAVA가 되어버릴 정도로 이제는 Sun의 상징이자, 세계적으로도 널리 알려진
단어가 되었다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=3)]

## 3. C, C++와의 비교 ¶

기존의 C에 객체 지향 기능을 억지로 끼워 맞추다 보니 영 모양새가 좋지 않은 [C++](C++.md)과는 다르게 아예 처음부터 [객체지향](OOP.md) 언어로 개발되었다. `[5]` C, C++, 자바의 차이점을 말하자면, C는 포인터 등을 활용한 로우 레벨 시스템
프로그래밍에 강점을 갖으며, C++은 C의 그런 강점을 거의 그대로 가져오면서 거기에 객체 지향과 같은 하이 레벨 기능들을 포함하였다.
문제는, 저수준 메모리 액세스를 허용하면서 하이레벨 기능들을 죄다 포함하려다 보니 디자인적인 측면에서도 좋은 소리를 못 들었다. 실제로
상당히 복잡한 언어가 되어 버렸고, C++을 제대로 다룰 줄 아는 프로그래머는 거의 없다는 이야기가 널리 퍼지게 되었다.`[6]` 자바는
여기서 포인터라는 강력한 무기를 포기한 대신에 OOP와 같은 하이 레벨 부분에 보다 집중하여 언어적 완성도를 높혔다 볼 수 있다.

  

일단, 대부분의 프로그래밍 언어가 그렇듯이, C와 비슷한 문법 구조를 가지고 있다. 그리고 명색이 고급 언어이기 때문에 C보다 생산성이 훨씬
더 좋다. 다만, [상속](%EC%83%81%EC%86%8D#s-2.md) 같은 객체 지향 개념을 이해하지 못하고 헤맬 경우엔
생산성과는 별개로 배우는 데 상당히 힘이 들 수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=4)]

## 4. 특징 ¶

자바의 가장 큰 특징은 플랫폼에 독립적인 언어라는 점. 소스코드를 머신코드로 컴파일하여 링크하는 C/C++과 달리 바이트코드인 클래스
파일(.class)을 생성하고, 이 파일을 일종의
[에뮬레이터](%EC%97%90%EB%AE%AC%EB%A0%88%EC%9D%B4%ED%84%B0.md)인 자바 가상 머신(=JVM)이
해석해서 실행한다. 이 특성으로 인해 자바는 태생적인 강한 장점과 심각한 약점을 모두 가지게 되었다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=5)]

### 4.1. 장점 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=6)]

#### 4.1.1. 비교적 높은 생산성 ¶

오늘날 프로그램의 덩치가 커지고, 다루는 것들도 크고 복잡해지면서 생산성과 퍼포먼스 문제가 생기게 되었는데, 로우 레벨 언어는 생산성이 너무
떨어지고 관리도 힘들어서 프로그램이 커지면 커질 수록 작업이 힘들어지게 되고, 아무리 컴퓨터 하드웨어가 발달한다고 해도 성능이 더 좋아지면
'빨라졌어? 그럼 이것도 할 수 있겠네'라고 해서 점점 더 복잡한 것을 다루고, 그게 또 표준이 되면서 하드웨어의 속도 향상이 무색해지기
때문. 거기다 리소스를 많이 낭비하는 하이 레벨 언어라면 더 심각하다.  
그런데, 그 와중에 나타난 게 바로 자바다. C언어와 비슷한 문법으로 진입 장벽도 낮고, 객체 지향을 적극적으로 이용하여 로우 레벨 작업들은
자동으로 처리해 주는 하이 레벨 언어이면서, 퍼포먼스도 다른 하이 레벨 언어들에 비해 빠른 편이다. 더욱이 호환성까지! 등장하자마자 순식간에
대세가 된 것도 무리는 아니다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=7)]

#### 4.1.2. 기기 호환성 ¶

장점으로는, 해당 [운영체제](%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C.md)에 [자바 가상머신](%EC%9E%90%EB%B0%94%20%EA%B0%80%EC%83%81%20%EB%A8%B8%EC%8B%A0.md)을 설치하면
자바로 만든 프로그램은 **어떤 컴퓨터에서도 완벽히 똑같이 동작한다.** 가상 머신이 각각의 운영체제에 맞춰서 결과적으로 완벽히 똑같이
돌아갈 수 있도록 제작되는 덕. 가상 머신 없는 운영체제라면 아예 자바 프로그램을 사용하지 못하겠지만, 썬마이크로시스템즈는 거의 모든 OS에
대해 가상 머신을 지원하고 있어서 이 부분은 보통 단점으로 꼽히지 않는다. 오히려 여러 운영체제에 발벌리는 업체라면 윈도우용, 맥용 등을
따로 제작할 필요 따위가 없이 **그냥 하나 만들면 끗!**이라고 자바 초창기 홍보되었다.`[7]``[8]`

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=8)]

#### 4.1.3. 안정성 ¶

그 이외에도 다른 로우 레벨 언어에 비해 높은 안정성을 꼽고 있다. 우선 C나 C++에 안정성 문제가 제기되는 포인터 연산자 및 메모리
직접접근 함수들을 지원하지 않는다. 여기에 C++과는 다르게 다중 [상속](%EC%83%81%EC%86%8D%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%29.md)을 허용하지 않는다. 이는 객체지향의 특성 중 하나인 '상속'의
자유도를 확 떨어트리는 것이기에 언뜻 보기에는 객체지향적 관점에 위배되는 것처럼 보일 수 있으나, 반대로 오히려 이게 더 객체지향적이라고 볼
수도 있다. 객체지향의 목적 자체가 재사용을 통한 생산성의 향상과 관리 상의 이점인데, 다중 상속은 잘못 사용할 시 극도로 복잡하게 꼬인
프로그램을 만들 위험성을 갖고 있다. 물론 코드 관리의 측면에서도 이는 좋지 못하다. 수준 높은 프로그래머라면 이 문제도 잘 해결할 수
있지만, 아예 미연에 방지해버리기 위해 다중상속을 언어 상에서 제거하는 게 안전성 면에서는 더 좋을 것이다. 어차피 자바에서는 다중 상속을
포기함으로써 생기는 문제를 interface를 다중 구현할 수 있도록 하여 어느 정도 해결했기도 하다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=9)]

### 4.2. 단점 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=10)]

#### 4.2.1. 속도 문제 ¶

이 방식으로 인해서 동시에 나온 자바의 심각한 단점은, 실행하는 과정에서 가상 머신을 **반드시** 사용해야 해 로우 레벨 언어에 비하면
느린 편이다 `[9]`. 하지만 요즘 같은 고사양 컴퓨터에서는 많은 라이브러리를 끌어오는 것이 아니라면 체감 상 차이는 없다. 다만
[운영체제](%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C.md)와
[게임](%EA%B2%8C%EC%9E%84.md)같이 퍼포먼스와 자원관리가 매우 중요하거나`[10]` 시스템을 성능을 한계까지 요구해서
직접 다뤄야 하는 프로그래밍은 하기 힘들다.`[11]` 가상 머신도 프로그램이고, 부담을 주는데 시스템 하드웨어의 **모든** 성능을
한계까지 끌어낼 수 있을 리가 없다. <del>그래서
[마인크래프트](%EB%A7%88%EC%9D%B8%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8.md)가 렉이 많이
걸렸냐</del>

  

이런 문제점을 제작자 본인들도 알고 있어서, 그런지 현재 쓰는 자바 가상 머신은 느린 인터프리터는 초기 동작에서만 쓰고, 그 다음에는 이미
인터프리터로 해석해놓은 기계어 코드를 기억해놨다가 바로 써서, 사용자 인터페이스가 보이지 않는 서버 프로그램은 실행 속도가 거의 기계
전용으로 컴파일된 언어에 필적하는 경우도 흔하다.`[12]` 하지만, 그만큼
[메모리](%EB%A9%94%EB%AA%A8%EB%A6%AC.md)가 뒷받침해줘야 한다.

  

또한 Swing이나 SWT를 이용해서 상용규모의 GUI프로그램만 만들어도 심각하게 느리다는걸 체감할 수 있다.

  

이 때문에 퍼포먼스가 매우 중시되는 분야에서는 네이티브 컴파일이 되는 [C](C.md), [C++](C++.md) 등을 쓰는게
일반적이다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=11)]

#### 4.2.2. 불편한 예외 처리 ¶

그리고 프로그램을 돌리다가 프로그램이 의도된대로 동작하지 않는 상황에서 예외를 발생시켜 처리를 할 수 있다. 대부분의 언어에서 차용하고 있는
좋은 기능이지만... 유독 Java는 다른 언어와는 달리 **프로그래머 검사가 필요한** 예외가 등장한다면 무조건 프로그래머가 선언을 해줘야
한다. 그렇지 않으면 **컴파일조차 거부한다.** 원래 의도는 철저한 예외 처리를 하니까 만약에 발생할 수 있는 모든 상황에 안정성을 확보할
수 있겠지...였으나, 결국 많은 경우엔 **조낸 귀찮다**는 이유로, 가장 일반적인 예외 하나만 써서 처리 안 하고 폭탄 돌리듯 넘기기만
하거나, 예외 나든 말든 무시해 버리는 경우가 가장 흔하다`[13]`. 이런 코드가 너무 흔해 빠진 나머지 이딴 식으로 쓸 거면 왜 넣었냐고
까는 사람도 많다. 그런데 선언 필요없는 **검사 안하는** 예외도 Java에 많다.(...)`[14]` 그리고 C++이나 C#같이 예외가
있는 언어라도 Java처럼 예외를 쓰는 경우는 별로 없다. 두 언어는 모든 예외가 **검사 안하는** 예외이다. 사실 예외 처리를 한다는
것은 귀차니즘과 견고함을 맞바꾸는 일인데, 안할 사람은 문법으로 강제해도 안한다는 것을 보여준다(..)

  

대부분의 다른 언어에서는 원하는 에러만 try-catch문으로 뽑아내고 그렇지 않은 경우에는 그냥 아무 처리를 해주지 않아도 된다. 이러한
언어를 접하던 사람이 자바를 접하면 그 특유의 경직된 예외처리에 불편해하기도 한다.

  

오히려 명시적으로 예외처리를 할 수 없는 경우도 존재하는데, 인터페이스를 상속받을 때 인터페이스에 선언된 예외가 아니면 구현클래스에서 그
예외를 던질 수 없다! 특히, 자바에서 제공하는 Iterator 인터페이스에는 throws 선언 따위는 없기 때문에 Iterator를
구현받았을 때 명시적으로 예외를 던질 수 없다. 이 상황을 해결하려면 RuntimeException 계열을 쓸 수밖에 없는 상황이 펼쳐진다.
<del>일종의 [의도는좋았다](%EC%9D%98%EB%8F%84%EB%8A%94%20%EC%A2%8B%EC%95%98%EB%8B%A4.md)인가</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=12)]

#### 4.2.3. 표준 입출력 지원 미비 ¶

기본적으로 자바는 콘솔 입력 함수를 제대로 지원하지 않는다. c에서 쓰이는 scanf와 같은 기본적인 입력함수를 제공하지 않고, 이것을
사용하려면 입력 스트림을 열고 예외처리를 하고 여러가지의 단계를 거쳐야 한다. c에서 한 줄로 끝나는 작업이 JAVA에 와서는 몇 줄 이상의
코드를 써야 하는데다가`[15]`, 그나마도 제약이 많다. 이 때문에 시중에서 판매중인 대부분의 자바 언어 책에서는 이 입력함수 구현 부분을
거의 거론하지 않고 있고, 대부분의 언어 입문서에서 가장 기본적이고 초반에 다루는 입력 함수를 통한 변수 입력 같은 파트가 없으며,
코드상에서 미리 입력된 변수를 통해 <del>혹은 main() 호출시 args로 준다던가</del> 예제를 구현하는 것으로 그친다. 물론
Java의 경우 GUI환경에서 사용되는 것을 상정하고 만들어졌기 때문이라고 생각할 수도 있지만, 달리말하면 언어가 지나치게 까다롭다는 말이
된다.[* 이 부분은 Java 5.0 이후로 [java.util.Scanner](http://download.oracle.com/javase
/1.5.0/docs/api/java/util/Scanner.html) 객체가 추가되면서 그나마 많이 편해졌다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=13)]

#### 4.2.4. 언어적 불편함 ¶

퍼포먼스 측면에서도 까이는 자바이지만 요즘 추세가 생산성을 극대화 시키는 것이다 보니까 최근 대세가 되는 고수준 언어들에 비해서는 생산성이
높다고 볼 수는 없다. 다른 고수준 언어(C#, python, ruby 등)에 비해서 문법적 설탕(syntactic sugar)이 적어서
이쪽에서 넘어오면 꽤 불편해하는 편.  
하지만 최근 Java8로 넘어오면서 람다 표현식, stream `[16]` 등을 지원하는 식으로 문법적 편리함을 늘려가는 추세이다. 이
흐름은 다음 java9 에서 더욱 강화될 것으로 보는 추세. <del>그래서 언제 나온답니까</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=14)]

##### 4.2.4.1. 연산자 재정의 미지원 ¶

그 의미가 명백할 경우에는 메소드 이름보다는 연산자로 나타내는게 훨씬 가독성이 좋다. 일례로 [C++](C++.md)에서 동적 배열인
std::vector같은 경우에는 선언한 뒤에 배열첨자(`[0]`, `[1]`)로 원소들을 직접 접근할 수 있다. 그러나 자바에서
ArrayList를 만들고 나면 항상 get이라는 메소드를 사용하여 원소에 접근해야한다. 코드가 길어질 경우 의외로 가독성에 영향을 주는
요소 중 하나.

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=15)]

##### 4.2.4.2. 명사형 생각을 강제 ¶

자바는 모든 동작이 객체 상위에서 이루어지게 함으로써 명사형으로 생각하는 것을 강제한다. 그 결과로 자바에는 전역 함수가 없고 모든 함수는
어떤 클래스에 종속되어있다. 이 때문에 기능적인 부분을 작성하는데 자잘한 클래스들을 작성해야 한다는 불편함이 있다.

  

이런 명사 중심적 생각은 확실히 많은 경우 편리하나 동사 중심으로 생각해야하는 상황도 생각보다 흔하다는게 문제. 예를 들어서, 퀵소트를
자바에서 엄격하게 의도된 대로 짜려면 QuickSort(array)라는 함수 대신에 Quicksorter라는 오브젝트의 생성자에 배열을 넣고
run()을 호출하여 동작을 하게 해야 하는 것이다. <del>물론 static을 써도 되지만</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=16)]

##### 4.2.4.3. [클로저](%ED%81%B4%EB%A1%9C%EC%A0%80.md) 미지원 ¶

명사형 생각을 강제 한다는 것의 연장선. 자바에서 함수는 일급 객체로 취급되지 않는다. 어떤 '동작'을 넘겨야 할때는 그 동작을 추상화한
인터페이스를 만들고 -> 그것을 구현한 뒤 -> 객체를 파라미터로 넘겨야한다. 반면에 클로저를 지원하는 언어는 그냥 함수를 파라미터로 넘기면
된다.  
Java8 에서는 람다 표현식을 지원함과 더불어 Function, 즉 함수를 멤버 표현이라는 방식(this::add) 으로 다른 함수의
파라미터로 넘길수도 있다. 다만 이 역시 자유롭지 못하고 파라미터로 넘겨지는 함수의 매개변수, 반환형이 단 한개씩으로 정해져 있어야 하며
void 형의 (리턴이 없는) 반환형을 지원하지 않는다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=17)]

### 4.3. 기타 ¶

또한 자바에서 UI를 만들 때도 고려를 해야할 게, 자바는 UI를 만들 때 AWT나 SWING 둘 중 하나 혹은 둘 다 선택하여 UI를
만드는 게 가능하다. 조심해야 할 점은, AWT로 생성한 UI는 SWING UI에 가려버린다. 그래서 멀정히 잘 돌아가는 코드인데도 불구하고
배경이 컨트롤(콤보박스라거나)을 가려버리는 일이 있을 수 있다.<del>그러므로 API는 통일해서 개발합시다.</del>

  

가비지 컬렉션을 제공하여 개발자가 직접 메모리의 할당과 해제를 관리해야 할 일이 없지만, 고급 주제로 넘어가면 가비지 컬렉션의 동작 원리를
이해해야 함과 동시에 할당과 해제 사이클을 직접 제어해야 하는 모순적인 상황 또한 제공한다.

  

자바 클래스 바이트 코드 매직넘버가 0xCA 0xFA 0xBA 0xBE다. 이것을 붙이면 CAFEBABE 다. CAFEBABE인 이유는,
제임스 고슬링과, 다른 연구원들이 St. Michael's Alley 라는 곳에 [점심](%EC%A0%90%EC%8B%AC.md)을
먹으러 가곤 했었다고 한다. 그 지방 전설에 의하면 그곳에서 [Greatful Dead](Greatful%20Dead.md)라는
[밴드](%EB%B0%B4%EB%93%9C.md)가 크게 성장하기 전에 연주하던 곳이라고 했다. 제리가 죽었을때,
[불교](%EB%B6%88%EA%B5%90.md)같은 신사를 세웠다고 한다. 그리고, 제임스 고슬링과, 연구원들은, 그곳을 Cafe
Dead 라고 불렀다. 그러다, CAFE DEAD 가 헥스 넘버인것을 알아냈다고 한다`[17]`. 그때 마침, 그는 파일 포멧 소스와,
메직넘버를 개편하고 있었다 `[18]`. 결국은, Object [파일](%ED%8C%8C%EC%9D%BC.md)의 메직 넘버는
CAFEDEAD 가 됬다. 나머지 하나, 클래스 파일의 메직넘버는 CAFE다음에 맞을 만한 번호를 정하는 것인데, 그때 적은 것이 BABE
다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=18)]

## 5. 변종 및 개발환경 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=19)]

### 5.1. 개발환경 ¶

자바에 특정한 라이브러리를 가미해서 웹에서 돌릴 수 있게 한 것이 **[자바애플릿](%EC%9E%90%EB%B0%94%20%EC%95%A0%ED%94%8C%EB%A6%BF.md)**이다. 애플릿 특유의 제약으로
인해 [ActiveX](ActiveX.md)보다는 훨씬 안전하다는 이유로 물 건너에서는 인터넷 뱅킹이나 결제용도로 사용하기도 한다.
근데 상대적으로 안전하다는 것일 뿐, 애플릿을 사용한 결제시스템도 툭하면 뚫려서 문제가 발생하곤 한다(…). 더군다나
[아이폰](%EC%95%84%EC%9D%B4%ED%8F%B0.md)과
[안드로이드](%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C.md)에서는 되지 않는다.

  

웹 어플리케이션 제작을 위해 자바 언어를 사용하는 규격으로 자바 서블릿과 [JSP](JSP.md)(자바 서버 페이지)가 있다.
`[19]` 주로 기업에서 사용한다. 개인 웹호스팅에서는 이를 지원하는 경우는 많지 않다.

  

썬/오라클에서 제공하는 Java Development Kit(자바 개발 도구)를 설치하면 javac란 컴파일러가 제공된다. 하지만 통합 개발
환경(=IDE)은 제공해 주지 않기 때문에, 반드시 별도의 개발용 프로그램을 써야한다. 대표적으로 이클립스, 넷빈즈, 인텔리J 등이 있다.
만약 이것을 안 쓰겠다고 한다면, 당신에게는 메모장과 javac.exe가 있을 뿐이다. 그리고 자바는 [IDE없이 타이핑만으로짜기엔](%EB%82%A0%EC%BD%94%EB%94%A9.md) 굉장히 불편한 언어라는 것을 명심하자. `[20]`
<del>import문, 변수 타입, try-catch문 쓰다가 [으앙주금](%EC%9C%BC%EC%95%99%20%EC%A3%BC%EA%B8%88.md)</del>

  

실전 자바 개발을 할 때 프로젝트에 필요한 라이브러리 관리나 프로젝트 결과물 배포 등 프로젝트 빌드 관리를 위한 도구로는 아파치 재단에서
만든 Ant와 Maven이 많이 사용되고 있다. 최근에는 이 두가지의 단점을 보완한 Gradle이 각광을 받고 있으나 국내에는 아직 많이
쓰이지는 않는 듯 하다.  
통합 개발 환경 프로그램으로는 이클립스 재단에서 만든 이클립스가 가장 많이 사용되는 편이고, 그 밖의 지명도 있는 것으로는 썬에서 만든
넷빈즈나 제트브레인 사의 IntelliJ IDEA 등이 있다. 자바가 꽤 오래 인기가 있었던 언어이고 많이 사용되어온 언어이기 때문에, 위에
나열한 것 외에도 정말 많은 도구가 사용된다.(...) <del>언어보다 도구사용법 익히는 시간이 더 오래 걸린다
[카더라](%EC%B9%B4%EB%8D%94%EB%9D%BC.md).</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=20)]

### 5.2. 다른 언어 같은 출력물 ¶

이외에 자바와 똑같이 자바바이트 코드를 생성하지만 언어 규격이 다른 [Scala](Scala.md)와
[Clojure](Clojure.md)라는 언어들도 있다. [Scala](Scala.md)는 'Scalable
Language'에서 따왔는데, 자바와 비슷한 부분이 많으며 자바 API를 그대로 가져다 쓸 수도 있다. 또한, syntactic
sugar가 많고 [함수형 프로그래밍](%ED%95%A8%EC%88%98%ED%98%95%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D.md)의 여러가지 요소들을 가져와서 자바에 비해 생산성도 높다. 일례로 일일히 타입 추론을 var
x = 1.5와 같이 넣으면 알아서 float 형으로 추론해준다. `[21]` 또, switch-case의 확장판이라 할 수 있는 패턴
매칭을 지원하며 클로저도 지원된다. 단점으로는 이런 고수준-고생산성의 언어에서 많이 볼 수 있듯이 같은 자바 코드에 비해 약간 느리다.  
[Clojure](Clojure.md)는 Java 플랫폼에서 동작하는 [LISP](LISP.md) 방언으로 설계되었으며
Common Lisp와 Scheme과 함께 주요 LISP 방언 중 하나로 꼽힌다. 이 언어도 마찬가지로 자바 API를 가져다 쓸 수 있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=21)]

### 5.3. 자바로 구현한 다른 언어 ¶

  * Jython : 파이썬을 자바로 구현한 언어 구현체. 따라서 Java 클래스와의 접합성이 좋으며 Java의 기본 제공 클래스들을 가져다 쓸 수 있다. 참고로 로고는 Java의 커피 컨셉과 Python의 뱀 컨셉을 섞어서 커피잔에서 [뱀](%EB%B1%80.md)이 연기처럼 피어나오는 로고이다(..)
  * JRuby : [루비](%EB%A3%A8%EB%B9%84.md)의 대부분을 자바로 구현한 언어 구현체.
  * Rhino: 자바에서 돌아가는 자바 스크립트이다. 모질라 재단이 100% 자바로 개발했다. 자바 스크립트를 사용하면서, 자바의 API를 사용하면서 자바 프로그램을 개발할수 있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=22)]

### 5.4. 유사품에 주의합시다 ¶

  * **유사품 A : [자바스크립트(JavaScript)](JavaScript.md)**  
자바스크립트는 이 자바와는 이름 말고는 언어 성격 상 연관성은 <del>마치
[너구리](%EB%84%88%EA%B5%AC%EB%A6%AC.md)와
[오리너구리](%EC%98%A4%EB%A6%AC%EB%84%88%EA%B5%AC%EB%A6%AC.md)의 관계처럼</del> 희박한
편이다. 자바를 가져다 변형한 수준도 아니다. 비슷한 건 문법의 일부 뿐이고 `[22]` 사용되는 라이브러리나 개념은 많이 다르다. 기초
패러다임상 당연한 요소들을 제외하고 나면 둘의 유사점은 오직 객체지향 뿐인데 그 마저도 자바스크립트는 프로토타입 베이스라 클래스를 쓰는
자바와 많이 다르다. 또 자바는 [컴파일](%EC%BB%B4%ED%8C%8C%EC%9D%BC.md) 언어이지만
[자바스크립트](JavaScript.md)는
[인터프리터](%EC%9D%B8%ED%84%B0%ED%94%84%EB%A6%AC%ED%84%B0.md) 언어다.`[23]`  
이처럼 이상한 관계가 된 이유는 넷스케이프 사에서 자기들이 만든 브라우저에서 자바스크립트를 탑재할 때 Sun하고 협력 관계를 가진 적이
있었기 때문. 그 때 자바가 소위 웹에서 '뜬다'는 언어라서 이름빨 좀 받아보려고. 그렇게 이름만 따다 붙인 것이다. 판권도 Sun과 아무
상관없다. 이름 하나 생각없이 잘못 붙여서 여러 사람 지금도 헷갈리게 만든 대표적인 케이스. 엄연히 **[자바와는 다르다, 자바와는!!](/
wiki/%EC%9E%90%EC%BF%A0%EC%99%80%EB%8A%94%20%EB%8B%A4%EB%A5%B4%EB%8B%A4%20%EC%
9E%90%EC%BF%A0%EC%99%80%EB%8A%94)**  
떠도는 말로 '자바와
[자바스크립트](%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md)의 차이는
[인도](%EC%9D%B8%EB%8F%84.md)와
[인도네시아](%EC%9D%B8%EB%8F%84%EB%84%A4%EC%8B%9C%EC%95%84.md)의 차이와 같다'라고도 한다.
간혹 인도와 인도네시아의 차이를 이걸로 설명하는 사람도 있다. <del>응?</del> 이 외에도, '자바와
[자바스크립트](%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md)는
[햄](%ED%96%84.md)과 [햄스터](%ED%96%84%EC%8A%A4%ED%84%B0.md)와 같은 관계이다'라는 표현도
있다.  
참고로 이 자바스크립트의 표준안에 대한 정식 명칭은 **ECMAScript**다.  

  * **유사품 B : Visual J++/Visual J#**  
Visual J++은 [마이크로소프트](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8.md)에서 자바를 변형하여 윈도우 전용으로 만든 언어. 위의 자바스크립트는 이름만 바꿨지만 이건 자바 자체를 윈도우에
맞도록 변형한 것이다. 이 때문에 자바 가상머신 없이 윈도우에서 네이티브로 돌아가지만, 다른 플랫폼에서는 전혀 돌아가지 않는다. 거기다 썬
마이크로시스템즈의 허락없이 마구 변형해서 썼기 때문에 소송크리를 먹고 개발이 중단되었다.
[망했어요](%EB%A7%9D%ED%96%88%EC%96%B4%EC%9A%94.md)  
이후 윈도우의 프로그램이 닷넷으로 넘어가면서 닷넷 기반의 Visual J#도 만들었다. Visual Studio 2005에 포함되었지만
이것도 개발이 중단되었다. 이때는 썬이 소송하지도 않았는데 중단된 것을 보면 시장성이 없었던 듯 하다. <del>결국은
[흑역사](%ED%9D%91%EC%97%AD%EC%82%AC.md)</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/Java?action=edit&section=23)]

## 6. 여담 ¶

자바의 창시자인 [제임스고슬링](%EC%A0%9C%EC%9E%84%EC%8A%A4%20%EA%B3%A0%EC%8A%AC%EB%A7%81.md) 옹은 진성
[애플빠](%EC%95%A0%ED%94%8C%EB%B9%A0.md)이다. 집에서 쓰는 IT 기기에 대해 묻는 질문에 폰, 타블렛,
데스크탑, 랩탑 등 거의 모든 IT 기기를 애플사 제품으로 도배해놨음이 밝혀졌다. 가족들도 마찬가지. 정작 애플은 OS X 레오파드 업데이트
때 자바를 찬밥 취급했지만...  
<del>그 뿐만 아니라 [공항에서 소시 자켓을 입고 인증을 찍는](http://jongkwang.com/?p=364) 레벨의
[소덕](%EC%86%8C%EB%8D%95.md)이다카더라.</del>`[24]`  
소덕이라 알려진 분은 제임스 고슬링이 아니라 프랑스에서 공연 기획 관련 일 하시는 분으로 예전에 KPOP관련 TV프로그램에서 인터뷰도 나온
그냥 닮은 분일 뿐 낚이지 말자.

  
  

제임스 고슬링과 자바 창시할때 같이 일했던 패트릭 노튼은 1999년 [FBI](FBI.md)의
[아동포르노](%EC%95%84%EB%8F%99%ED%8F%AC%EB%A5%B4%EB%85%B8.md) 함정수사로 인해 체포되었다.
`[25]` 덤으로 IT 관계자들은 노튼이 왜 [기업 방화벽을 통과할수 있는 통신도구를 만드는 일에 관심을 보인이유](%ED%8F%AC%EB%A5%B4%EB%85%B8.md)를 일찌감치 짐작했었다고...

  

조엘온 블로그로 유명한 [조엘](%EC%A1%B0%EC%97%98.md)이 엄청나게 싫어하는 언어.
[외부링크](http://openlook.org/blog/2005/06/04/cb-931/) 조엘 스폴스키가 자바를 싫어하는 이유로는
성능상의 문제나 문법상 너무 쉽다(...)`[26]`는 이유도 있지만, 자바 자체가 "위원회 기술"이라는 이유도 큰 몫을 차지한다. 사실
이는 자바가 가진 태생적 문제인데 자바라는 언어가 C#처럼 어느 특정 단체나 회사가 주도적으로 끌고가는 물건이 아니다 보니 위원회를 구성하는
각 업체들의 파워게임에 따라 중요한 문제의 해결방안이 빨리 처리 되지 않는 경우도 있고 배가 산으로 가는 경우도 있다. 더 심각한 점은,
위원회를 구성하는 업체들이 승질 나서 자기 멋대로의 자바 언어를 만드는 경우이다. 이 경우 자칫하면 똑같은 자바 코드인데 업체별 자바
가상머신에 따라 프로그램이 작동할 수도 안할 수도 있다.(...)

  

2012년 말, 자바에 보안 취약점이 발견되어 오라클에서 긴급 보안 패치를 발표했지만 또 다른 취약점이 발견되고 있다. 그래서 자바를 계속
써야 하나 말아야 하는 <del>[키배](%ED%82%A4%EB%B0%B0.md)</del>논쟁이 벌어지고 있다고 한다.<del>사실
자바에서 보안 취약점이 없던 때는 없다 카더라</del>

`\----`

  * `[1]` 창시한 사람은 제임스 고슬링 이다.
  * `[2]` 개발진이 자바산 커피를 좋아해서 그랬다는 설도 있다. 마크도 커피잔 모양.
  * `[3]` 개발자의 이름인 James Gosling, Arthur Van Hoff, Andy Bechtolsheim의 머릿글자를 따온 것이라는 설도 있다.
  * `[4]` 그냥 사전을 펼쳤는데 눈에 들어온 이름이었다는 설도 있다.
  * `[5]` 많은 사람들이 착각하는 부분인데, 자바는 엄밀히 말하면 완벽한 객체지향 언어가 아니다. 프리미티브(primitive) 타입은 객체로 취급하지 않기 때문. 모든것을 객체로 취급하는 언어를 순수 객체지향(pure object oriented)이라 하며 이를 지원하는 언어는 [Smalltalk](Smalltalk.md)가 대표적이다. 최근 만들어진 언어중엔 [C#](C%23.md)이 이에 해당된다.
  * `[6]` 실제로, [리누스 토르발스](%EB%A6%AC%EB%88%84%EC%8A%A4%20%ED%86%A0%EB%A5%B4%EB%B0%9C%EC%8A%A4.md)가 C++을 비판하면서 프로젝트에 C++이 아닌 C를 사용하는 이유 중 하나는 C가 좋아서라기보다 C++ 프로그래머들을 의도적으로 배제하기 위해서라고 한 적이 있다. C++의 경우, 고도로 숙련된 프로그래머가 주의 깊게 디자인하고 프로그래밍하지 않을 경우 망측한 코드를 만들어낼 가능성이 매우 높아 제대로 디자인된 언어가 아니라고 주장하였다.
  * `[7]` 그러나 다른 크로스 플랫폼 언어들과 마찬가지로 각 플랫폼마다 미묘하게 기능이나 작동에 차이가 있기 때문에 그러한 수정을 거치지 않고 한 플랫폼 용으로 만든 프로그램을 그대로 다른 데에서 돌리는 것은 사실상 허상이다. 처음부터 공통되도록 설계하거나 각 플랫폼에 맞추어 버전을 만드는 것이 보통. 작동이 다른 것으로 한가지 예를 들면 윈도우에서는 파일을 읽어올 때 파일 경로에 \ 를 사용해도 되지만 이렇게 짤 경우 리눅스에서는 동작을 안한다. 물론 레퍼런스에서는 \보다는 File 클래스의 separator를 사용하는 것이 권장되므로 이것만 가지고 문제삼는 건 옳지 않다.
  * `[8]` Java의 모토는 Write once, run everywhere인데 프로그래머들은 이를 비꼬아 Write once, **test** everywhere라고 말하곤 한다. <del>테스트라도 되는 게 어디야</del>
  * `[9]` 예전에 선 마이크로시스템이 자바 프로세서라는 자바 바이트 코드를 실행시키는 CPU를 만든다고 했었다. 자바 바이트 코드를 CPU의 명령어 (mov rax, 1;mov rbx, 1;int 0x80 같은 어셈블리어)를 실행시키듯이 네이티브로 돌리면 가상머신에서 돌아가는것보다 20배는 더빠르다. 근데 선은 실패했는지, [흑역사](%ED%9D%91%EC%97%AD%EC%82%AC.md)로 남게되었다.
  * `[10]` OS 프로그래머 중에는 C 언어를 하이 레벨 언어로 생각하는 사람도 종종 있다.
  * `[11]` 실제로 Sun에서 JavaOS를 만들기도 했지만, 흑역사이다.
  * `[12]` 이 바이트코드 컴파일러를 JIT이라고 부른다. 서버 모드일 경우는 무조건 JIT으로 컴파일이 기본값. 그 외에는 (VM에 따라 다르지만) 2~10번 정도 불려져야 JIT가 돌아가는 모드가 기본값이다.
  * `[13]` 물론 이렇게 짜면 안되지만 구조적으로 강요받는 형편
  * `[14]` 이쪽은 RuntimeException 계열의 예외로, 이것을 던지는 메소드가 throws에 명시적으로 던진다고 선언하지 않았을 경우 검사를 하지 않아도 된다.
  * `[15]` 어거지로 한 줄에 넣을 수는 있다. String str = new Scanner(System.in).nextLine(); 한 줄 밖에 못 읽는 단점이 있지만
  * `[16]` 컬렉션(Collection)의 이터레이터를 확장해서 처리할 수 있는 개념으로, 이터레이터의 원소를 필터링해서 원하는 원소만 뽑거나, 원소갯수를 줄여버리고, 이렇게 다시 뽑혀진 원소들로 갖가지 처리를 만드는 등 '함수적인(functional)' 기능을 제공한다
  * `[17]` CAFEDEAD 를 0xCA 0xFE 0xDE 0xAD로 바꿨을 때의 얘기인듯 하다.
  * `[18]` 그때 필요한 메직넘버는 2개였다. 하나는 오브젝트 파일이고, 또다른 하나는 클래스 파일 메직넘버였다.
  * `[19]` JSP의 목적이 HTML 페이지를 동적으로 만들어내는 것이다. JSP 페이지는 자바 서블릿 코드로 변환되어 서버에서 실행되고, 이 HTML 결과를 브라우저에 보여준다. JSP 페이지는 HTML 페이지에 자바 코드가 포함되어 있는 식으로 되어 있는 경우가 많고, 이 점은 PHP, ASP.NET 등과 비슷한 편이다. 반면 자바 서블릿은 서버 쪽에서 하는 일에 관심이 많지만 출력에 대한 관심은 적다. 필요하다면 브라우저에 출력을 전혀 안 보낼 수도 있다. 최근에는 Server side script language로 HTML 페이지를 동적으로 만드는 식으로는 프로그래밍을 하지 않는다. JSP, PHP와 같은 Server side script language로는 서버에 있는 자원의 접근을 주로 하고(DB 연산, File 연산 등등) 화면에 보여주는 UI는 HTML/CSS/Javascript로만 한다. 이를 위하 Client side와 Server side에 통신이 필요한데 XHR(XML HTTP Request)를 이용한다. 이러한 프로그래밍 기법을 나타내는 표현이 REST내지는 Open API이다.
  * `[20]` Java는 현용 프로그래밍 언어 중에서는 Verbose한(장황한) 언어로 꼽힌다. 즉, 같은 의미인데 많은 타이핑이 필요하다. <del>[vim](vim.md)으로 짜고 있자면 새끼 손가락이 시려온다..</del>
  * `[21]` 알아서 타입을 추론해준다는 의미. Scala는 자바같이 static typed 언어다. 
  * `[22]` 문법조차 별로 비슷하지 않고 상당히 다르다.
  * `[23]` 그나마도 요즘은 둘 다 [JIT](JIT.md)로 통일되어가는 추세다. 참고로 자바스크립트에 JIT를 최초로 도입한 브라우저는 다름아닌 [크롬](%ED%81%AC%EB%A1%AC%28%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%29.md).
  * `[24]` 실제로 본인은 아니고 그냥 닮은 사람...
  * `[25]` 단지 징역을 살지는 않고 FBI에서 1년 근무하는 것으로 퉁쳤다.
  * `[26]` 진입 장벽이 낮아지면 그만큼 실력 없는 초보 개발자들도 많이 있기 때문.
