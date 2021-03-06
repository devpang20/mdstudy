# 프로그래밍 공부와 개요  

## 공부 접근법

- 질보다 양을 승부한다. 최대한 많은 코드를 작성하고 수정해본다.
  - 코딩은 공부가아니라 훈련 
- 기술 이해는 눈으로 하지 않고 반드시 관련된 예제를 작성한다. 
  - 안보고 코드를 쓸 수 있을 때 까지(이해든 암기든)
- 프로그래머가 목표라면 기술위주의 공부는 피해야 한다.
  - 언어는 중요한 것이 아니다.
  - 로직을 이해와 경험치를 쌓는게 중요하다.
  - 최신 언어와 프레임워크를 배워봤자 시간이 지나면 구식기술이 된다.
- 질문은 주로 [스텍오버플로우](https://stackoverflow.com/])나 구글링을 활용한다. 
  - 먼저 찾아보고 (사실 찾아보면 초보수준의 질의응답은 모두 있다.) 물어본다.
  - 기본 정보 습득은 공식홈페이지가 가장 좋다.
---
- github의 오픈 소스를 분석해보며 잘짜여진 코드를 많이 보도록 노력한다.
  - 오픈 소스를 받은 다음 분석하고 자신이 뜯어 고쳐보는 재미를 느껴본다.(코더를 벗어나 프로그래밍을 하기위해서는 만든걸 습득하는 걸 넘어서 배운걸 응용해보는 경험을 쌓는다.)
- 가장 중요한건 이론보다는 실기이므로 무언가를 만드려고 노력하면서 이론을 그때 그때 습득 및 적용하도록한다.
  - 예) 게시판을 만들기 위해 php 객체에 관한 지식을 공부하고(이미 배웠거나) 적용한다. 
- 기술이 어떻게 돌아가는지 분석한다.
  - 작게는 단순한 로직 분석부터 깊게는 메모리 단 까지 노력하면 베스트!
- 기본기가 닦인 이후에는 구글링을 통한 정보습득, 처리, 적용 능력이 실무에서 가장 중요하므로 자료 해석 능력을 기른다.

## 개요

프로그래밍은 코드, 데이터로 구성되어있다.

데이터는 말 그대로 데이터. 기본적으로 숫자, 문자가 있으며, 데이터를 담을 수 있는 배열, 객체 같은 데이터가 있다.
또 프로그래밍의 논리를 표현하기 위해 참, 거짓을 나타내는 데이터가 있다.
그리고 데이터가 없음을 나타내는 데이터인 null이 있다.

코드는 컴퓨터에게 명령을 내리는 것이다.

- 1과 1을 더해라: 1 + 1;
- 문자열을 HTML에 찍어라: echo '문자열';

따라서 코딩을 할 때에는 컴퓨터가 이게 코드(명령)인지, 데이터(값)인지 구분할 수 있어야 한다.

코드는 대개 특수기호와 의미 있는 단어들로 이루어져있다.

- 문자열을 찍게하는 echo
- php를 종료시키는 exit
- 두 숫자 데이터를 더하는 +
- 변수에 값을 대입하는 =
- 조건문인 if
- 반복문인 for
- 각 명령이 끝났음을 알리는 ;

프로그래밍이라는게 어차피 값을 계산하거나 무언가 글자를 보여주는게 목적이다. 따라서 데이터는 대개 숫자와 문자열이 대부분이다.
문자열은 코드와 구분되어야 한다.

- 숫자는 그냥 숫자 그대로 표현한다: 123, 555.123
- 문자열은 '' 또는 ""사이에 넣어 표현한다: "Hello" 'Hello'

프로그래밍은 데이터를 이용해 컴퓨터에 명령을 내리는 작업이다.
명령은 `논리`와 `반복`으로 이루어져있다.

- 이게 맞으면 뭘 해라(논리)
- 이걸 몇 번 반복해라(반복)
- 이게 무엇이면 몇 번 반복해라(논리 + 반복)

이런 논리, 반복을 나타내는 `if` `while` `for` 등이 있다.

프로그래밍은 이렇게 코드와 데이터를 이용해 컴퓨터에게 명령을 내리는 작업이다.
