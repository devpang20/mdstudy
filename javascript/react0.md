# 리엑트 기본 

## ES6+

### cosnt, let
- 기존 es5에서 변수는 var 로 선언했다. 하지만 es6 버전 부터는 const와 let을 사용할 수 있다
  
- var, let는 재할당이 가능하지만 const는 재할당이 불가능하다.
- 기본적으로 const로 선언하고 해당 값을 바꿔주어야 할 때는 let를 사용합니다.

```js
    let a = 1;
        a = 2; // error
  
    const b = 1;
    b = 2; //error
```

- JSX   
  - 자바스크립트 확장 문법
  - 작성문법은 번들링 되면서 bable-loader를 통해 자바스크립트 변환한다.
  - 준수해야하는 규칙
    - 컴포넌트 변화 감지를 위해 부모요소로 반드시 감싸야한다.

```js
import React, { Component } from 'react';

class example extends Component {
  render() {
    return (
      <div>
        <h1>부모요소로 감싸주어야합니다.</h1>
      </div>
    );
  }
}

export default example;

```