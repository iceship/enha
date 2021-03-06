[이스트소프트](%EC%9D%B4%EC%8A%A4%ED%8A%B8%EC%86%8C%ED%94%84%ED%8A%B8.md)에서
[알집](%EC%95%8C%EC%A7%91.md)의 [EGG](EGG.md) 포맷에 사용하기 위해서 만든 [무손실 압축 포맷](/
wiki/%EB%AC%B4%EC%86%90%EC%8B%A4%20%EC%95%95%EC%B6%95%20%ED%8F%AC%EB%A7%B7).

[알집](%EC%95%8C%EC%A7%91.md)에서 [EGG](EGG.md) 포맷으로 압축을 할때, 압축율과 압축 속도의
최적화를 위해서 파일의 [확장자](%ED%99%95%EC%9E%A5%EC%9E%90.md)별로 다른 압축 알고리즘을 사용한다. 예를
들자면 .txt 파일은 [bzip2](bzip2.md) 알고리즘으로 압축하고, .exe 파일은
[Deflate](Deflate.md) 알고리즘을 사용하는 식. 그런데 파일의 확장자가 .com이나 .sys 인 파일은 AZO
알고리즘으로 압축을 한다.

원래 알집 8.0 베타 버전(알집 EGG 에디션 이라고 불렸다)에서는 .DLL 파일을 AZO 알고리즘으로 압축을 했었는데, 압축 알고리즘이
너무 느린 관계로 파일의 크기가 매우 작은 .com , .sys 파일에 대해서만 AZO 알고리즘으로 압축을 한다.  

사실상 [EGG](EGG.md) 포맷이 LZMA 알고리즘을 지원하게 되면서 부터 AZO 알고리즘을 사용할 이유가 전혀 없지만, 굳이 이
알고리즘을 사용하는 이유는 다른 회사에서 EGG 포맷을 맘대로 압축을 해제하기 못하게 하기 위한 정책이 아닌가 의심된다.

AZO 알고리즘은 속도는 느리지만 압축율이 매우 뛰어난 알고리즘이다. 기본적으로 [ZIP](ZIP.md) 포맷에서 쓰이는
[Deflate](Deflate.md) 알고리즘보다 훨씬 뛰어난 압축율을 보여주고 있으며, 심지어 최강의 압축율을 지닌다고 알려진
[7zip](7zip.md)의 [LZMA](LZMA.md) 알고리즘과 버금가거나 더 좋은 압축율을 보여주었다. (파일의 확장자를
.com 으로 바꾸고 egg 포맷으로 압축을 해보면 실험이 가능하다)

압축율이 이렇게 뛰어난 이유를 분석하기 위해서 리버스 엔지니어링을 해본 결과.... [LZMA](LZMA.md) 와 거의 동일한 압축
방식을 사용하고 있는 것으로 보인다. ([LZ77](LZ77.md) 을 사용하는것은 확인되었고 백엔드로도 Binary Range
Coding을 사용하는 듯 하다.) <del>그럼 그렇지</del>

  

