## Contents

    

1. Solid State Hybrid Drive 
    

1.1. 개요

1.2. 문제점

1.3. 사용처와 장점

1.4. 기타

2. Secure SHell Daemon 

[[edit](http://rigvedawiki.net/r1/wiki.php/SSHD?action=edit&section=1)]

## 1. Solid State Hybrid Drive ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/SSHD?action=edit&section=2)]

### 1.1. 개요 ¶

[SSD](SSD.md)와 [HDD](HDD.md)의 특징을 합친 저장장치.

  

데이터 저장은 HDD에 SSD를 캐쉬로 이용, 자주 이용하는 데이터를 읽을 때는 SSD와 동등한 속도를 낸다. SSD 부분을 캐쉬처럼
이용하지만, 휘발성 램 캐쉬에 비해서는 속도가 느리므로 HDD와는 판이한 캐쉬
[알고리즘](%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98.md)이 필요하다. 2014년 현재 발매된 SSHD의
플래시램 용량은 8기가 정도이다. 32~64메가 정도에 지나지 않는 [HDD](HDD.md)의 캐쉬와 비교하면 매우 광활한 크기이다.
고속의 휘발성 램 캐쉬 역시 달린다.

[[edit](http://rigvedawiki.net/r1/wiki.php/SSHD?action=edit&section=3)]

### 1.2. 문제점 ¶

이렇게 쓰면 매우 좋은 기술 같지만 현실은 SSD만큼 비싸고 HDD만큼 느리다고 대차게 까인다. 제 성능을 발휘할 수 없는 까닭은 PC는
다양한 작업을 하므로 읽는 파일이 제각각이기 때문이다. SSD 캐쉬가 아무리 빨라도, 필요할 때 데이터가 캐쉬에 없으면 아무런 소용이 없다.

  

8기가 이상의 캐쉬는 기존보다 혁명적으로 크다. 이론상 캐싱
[알고리즘](%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98.md)이 제대로 작동한다면 SSD에 필적하는 빠른 속도를
기대할 수 있다. SSHD의 알고리즘은 복잡하게 구성되지만 간략하게 설명하면 이렇다. HDD의 성능을 저하하는 요소는 크기가 작고 숫자가
많으면서 읽기 빈도가 높은 저용량 파일이다. 이것은 SSD 캐쉬 영역에 놓아서 읽고 쓴다. 상대적으로 용량이 크고 읽기 빈도가 낮은 파일은
HDD 영역에서 읽고 쓴다. 이러면 두 매체의 장점을 살릴 수 있다. 그러나 실사용에서는 기대 성능이 나오지 않는다. 따라서 캐싱 알고리즘이
불완전하다고 짐작할 수 있다.

  

기술적인 면을 들여다보면 왜 제 성능이 나오지 않는지 짐작할 수 있다. 2014년 현재 SSD는 발매된지 10년 가까이되며, 계속 불안한
성능을 보였다가 최근 몇년 사이에 안정적인 제품이 나오는 형국이다. 컨트롤러가 SSD 기술의 핵심인데, 한때 다수의 컨트롤러 제조 회사가
난립하다가 현재는 적은 수의 회사 밖에 남지 않았다. 비메모리 반도체 기술로 이름 높은
[인텔](%EC%9D%B8%ED%85%94.md)이 컨트롤러 개발에 손을 땔 정도이니 생각보다 난이도가 높은 기술이다.

  

SSHD는 원리상 SSD와 HDD가 합쳐진 물건이다. 칩 설계가 주종목이 아닌 HDD 제조사가 원하는 성능의 SSD 컨트롤러를 개발하기도
어렵다. 다른 회사의 컨트롤러를 장착해도 SSD와 HDD 양쪽 모두 다른 알고리즘이 필요하다. 원하는 성능이 나올지 확신할 수 없으며,
제조비용도 오른다. 실상 SSHD의 알고리즘은 SSD 단독 알고리즘보다 훨씬 복잡하다. 이러니 성능과 가격을 타협한 제품이 나올 수밖에
없었으리라.  

[[edit](http://rigvedawiki.net/r1/wiki.php/SSHD?action=edit&section=4)]

### 1.3. 사용처와 장점 ¶

보급형 노트북은 설계에서 mSATA슬롯을 TV카드나 와이파이 칩에 배정한 경우가 많아 쓸 수 없는 경우도 많다. 이런 노트북 대상의 수요가
있다. 다만 SSD의 가격이 점점 내려감에 따라 이 마저도 흔들리고 있는 상황. WD는 2.5인치 듀얼드라이브같은 변태같은 물건을 내놓기도
했다.

  

데스크탑 사용자는 SSD와 HDD를 따로 구매하는 편이 효율적이다. OS나 프로그램 설치는 속도를 위해서는 SSD에, 데이터는 HDD를
사용하면 좋다.

  

고성능 노트북은 SSHD를 장착하고 출시되는 모델들이 있다. mSATA SSD 및 2.5인치 SSD의 고성능 스토리지를 적용시키기엔,기업들
입장에선 생산원가에 대한 부담이 큰 이유이다. 또한 노트북의 특성인 휴대성을 감안했을때 데스크탑과 같은 듀얼 스토리지 구성(SSD+HDD)은
제품의 총 중량을 높이는 이유로 자주 선택되는 옵션은 아니다

  

효용이 큰 분야는 콘솔 게임기 HDD 대용이다. 고용량 SSD는 콘솔 가격만큼 하므로 배꼽이 더 커진다. [PC](PC.md)보다 같은
파일을 더 자주 읽어야하는 콘솔의 특성상, SSHD의 알고리즘은 콘솔에 더 적합하기도 하다. [PS4](PS4.md)는 하드 교체가
쉽고 기본 용량 부족에 따른 교체 수요가 있어서, 이때 SSHD를 장착하기도 한다. 성능은 HDD와 SSD의 딱 중간 정도인듯. [#](ht
tp://www.bodnara.co.kr/bbs/article.html?D=7&cate=11&d_category=8&num=103814)

  

[애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md) 에서 사용하는 [퓨전드라이브](%ED%93%A8%EC%A0%84%20%EB%93%9C%EB%9D%BC%EC%9D%B4%EB%B8%8C.md) 와 비슷하다.
SSD 와 HDD 를 섞어놓은 형태. HDD 1TB, SSD 128GB 로 구성된다.

[[edit](http://rigvedawiki.net/r1/wiki.php/SSHD?action=edit&section=5)]

### 1.4. 기타 ¶

처음에는 Hybrid HDD (HHD)라는 명칭을 사용했다가, SSHD로 명칭이 바뀌었다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/SSHD?action=edit&section=6)]

## 2. Secure SHell Daemon ¶

  

서버에서 SSH 서비스를 제공하기 위해서, 동작하는 서버 데몬이다.
