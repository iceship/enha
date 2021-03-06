VHDL(VHSIC Hardware Description Languae)은 디지털 회로의 설계 자동화에 사용하는 하드웨어 기술
언어(hardware description language ,HDL)`[1]`, 즉 회로 설계 언어이다. 엄밀히 말하자면 [프로그래밍언어](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4.md)는
아닌데 어차피 요즘 차이가 점점 모호해지는 관계로 그냥 프로그래밍 언어 항목에 끼워넣은 듯 하다(?).

본래 개발목적은 미국 국방부에서 주문형 집적회로(ASIC = Application Specific Integrated
Circuit)`[2]`의 문서화에 사용하기 위하여 만든 언어이다. 복잡한 매뉴얼로 사용자의 [뇌](%EB%87%8C.md)를 아프게
하는 대신, 회로의 동작 내용을 문서화하여 설명하기 위해 개발된 것. 그런데 언제부터인가 이런 문서를 회로 디자인 과정에서의 시뮬레이션에
사용하게 되었고, 여기에 재미들려서 VHDL 파일을 읽어들여서 논리 합성 후에 실제 회로 형태를 출력하는 기능을 덧붙이게 되었다. 결국,
오늘날에는 디지털 회로의 설계, 검증, 구현 등의 모든 용도로 사용하는 중.

기본적인 베이스는 본래 [Ada](Ada.md)의 부분집합에 시간 개념(디지털 회로에 필수적인)을 추가하는 방식이었으나, IEEE
표준화 작업을 거치면서 오늘날과 같은 형태와 문법을 가지게 되었다.

[Verilog](Verilog.md)와 함께 대표적인 하드웨어 기술 언어이며, 최근은 대부분의 회사는 고유 포맷을 이용하기보다는 이
두가지 표준 HDL을 사용하는 추세.

`\----`

  * `[1]` 말 그대로 전자 회로를 정밀하게 기술하는데 사용하는 컴퓨터 언어. 시간과 동시성(concurrency)를 표현할 수 있는 표기법이 있다는 점, 컴파일 과정이 다르다는 점 등이 일반 프로그래밍 언어(즉 소프트웨어 프로그래밍 언어)와 다르지만, 요즘에는 reconfigurable system이라고 두 언어의 특징을 결합한 방식이 사용됨에 따라서 차이는 모호해지는 중.
  * `[2]` 특정한 용도로 사용하기 위한 집적 회로. 동작 속도 향상, 구현 면적 소형화, 소비 전력 감소 등의 장점이 있는 반면 설계가 어렵고 제조 공정 시간이 오래 걸리고 무엇보다 (소량 생산의 경우)개비싸다! 는 단점이 있다.

