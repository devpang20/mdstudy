- php 와 js 버전 모두 출력
- php의 경우 [실습페이지](https://repl.it/languages/php)
- js의 경우 브라우저 개발자 모드 활용 

---

## while을 통한 구구단 문제 

- while 문을 통해 구구단을 출력하시오.
  예상 결과값
  1단
  1 * 1 = 1  
  1 * 2 = 2  
  1 * 3 = 3  
  1 * 4 = 4  
  .  
  .  
  .  
  9단  
  9 * 8 = 81  

---

## for 문을 통한 구구단 문제 

- for 문을 통해 구구단을 출력하시오.
  1단  
  1 * 1 = 1  
  1 * 2 = 2  
  1 * 3 = 3  
  1 * 4 = 4  
  .  
  .  
  .  
  9단 
  9 * 8 = 81  
---

## 종합테스트 - 짝수 숫자만 구구단 출력

- 2, 4, 6 ,8 단만 출력하시오.
  
---

## 매개 변수 없는 함수 출력 문제 

- 함수를 실행하면 'hello'를 실행 하도록 함수를 만드세요

- php 정답
```php
    <?php
    function test(){
    echo 'php test 함수입니다.';
    }

    echo test();
    ?>
```
- js 정답

```js
  function test(){
    document.write('script test 함수입니다.');
  }
  test();
```
---

## 매개 변수 있는 함수 출력 문제 

- 매개변수가 있는 함수를 만들고 매개변수에 숫자를 입력 할때 때마다 "이것은 <매겨변수값> 입니다."라고 출력하시오.
  
php  
예)echo test(1)  
=>이것은 1 입니다.  

js  
예)test(1)  
=>이것은 1 입니다.  

---

## 매개 변수 있는 함수 출력 문제 2

- 매개변수가 있는 함수를 만들고 매개변수에 숫자를 입력 할때 때마다 매개 변수 값에 곱하기 2를 하는 함수를 출력하시오.
  
php  
예)echo test(2)  
=> 4   

js  
예)test(2)  
=> 4   

---

## 종합 테스트 구구단 출력 함수

- 함수 매개변수에 해당 숫자를 넣으면 구구단이 출력 되는 함수를 만드시오. 

php

예)echo gugudan(1)  
=>   1단
  1 * 1 = 1  
  1 * 2 = 2  
  1 * 3 = 3  
  1 * 4 = 4  
  .  
  .  
  .  

js  

예)gugudan(1)   
=>   1단  
  1 * 1 = 1  
  1 * 2 = 2  
  1 * 3 = 3  
  1 * 4 = 4  
  .  
  .  
  .  
