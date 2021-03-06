# 코드와 데이터

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

---

# 데이터 타입

프로그래밍은 코드와 데이터로 이루어져 있다고 했다.

그럼 어떤 데이터가 있는지 알아보자.

## 숫자

컴퓨터는 애초에 계산을 위해 만들어졌다. 따라서 자연스럽게 데이터형은 숫자가 있을 수 밖에 없다.
숫자는 정수형과 실수형이 있는데, 이는 정수형이냐 실수형이냐에 따라 컴퓨터 메모리에 저장하고 읽어오는 방식이 다르므로 확실히 구분해야 한다.

- `int`: 정수형
- `float`: 실수형

숫자는 그냥 숫자 그대로 표현한다.

- 정수 `123`: 123
- 실수 `1.5`: 1.5

## 문자, 문자열

문자와 문자열을 구분하는 언어도 있지만 php는 그렇지 않다. 문자나 문자열 모두 '', "" 안에 문자를 넣으면 된다.

- 문자열 `Hello`: 'Hello' 또는 "Hello"

''와 ""의 차이점은 언어마다 다르지만 php의 경우 ''은 안에 있는 모든 문자가 문자열로 표현되는 반면에, ""는 특수한 기호를 이용하면 데이터(변수)도 표현할 수 있게 해준다.

```php
$hello = 'Hello';
$world = 'World';

echo $hello . ' ' . $world; // Hello World
echo "{$hello} {$world}" // Hello World
```

결과는 같지만, 문자열 결합 연산자같은 `.`를 사용하지 않고 알아보기 쉽게 사용할 수 있다.
"" 안에서 변수를 사용할 때에는, 해당 변수를 {}로 감싸주면 가독성이 좋아진다. 사실 감싸지 않아도 되지만, 예를 들어 아래와 같은 경우

```php
$fruit = '오렌지';

echo "$fruit는 맛있습니다"; // 에러. '$fruit는' 자체가 변수명으로 인식된다.
echo "{$fruit}는 맛있습니다"; // OK
```

이렇게 변수에 글자를 이어붙여야 하는 경우에는 {}로 구분을 해줘야 하기 때문에, 그냥 모든 경우에 {}를 사용하면 혹여나 에러가 발생해도 그 에러를 애써 찾을 필요가 없어진다.

## boolean

프로그래밍의 논리를 표현하는 데이터이다. `true` `false`가 존재한다. 보통 `if`문 안에서 많이 사용한다.

`true`냐 `false`냐에 따라서 컴퓨터에게 명령을 다르게 내릴 수 있게 해준다.

## array

배열은 기본적으로 연속된 데이터들을 저장할 수 있는 데이터다.

```php
$arr = [1, 2, 3, 4, 5];
echo $arr[0]; // 1
```

이는 데이터를 효율적으로 관리할 수 있게 해준다.

한 교실에 있는 학생들의 기말고사 평균점수를 데이터로 다뤄보자. 학생들은 각자 자기의 번호가 있을 것이다.

```php
$student1 = 90;
$student2 = 100;
$student3 = 80;
// ...
```

이렇게 모든 데이터를 변수 하나하나에 저장하면 너무 귀찮고 불편할 것이다. 따라서 배열을 이용해보자.

```php
$students = [
  90, 100, 80, 70, // ...
];
```

프로그래밍에서 인덱스는 보통 0부터 시작한다. 따라서, 첫번째 데이터는 배열의 인덱스 0으로 얻어올 수 있다.

```php
$students[0]; // 90
```

이렇게 배열을 이용하면 연속적인 데이터를 효율적으로 갖고 있을 수 있다. 또, 인덱스값이 정수형이므로 다른 변수에 담겨있는 데이터를 이용해 배열의 인덱스를 표현할 수도 있을 것이다.

```php
$number = (int)$_GET['student_number'] - 1; // 클라이언트가 요청한 학생 번호를 가져온다.
                                            // 여기서 (int)는 숫자형태의 문자열을 숫자로 바꿔주는 역할을 한다.

echo "{$number}번 학생의 성적은 {$students[$number]} 입니다.";
```

php의 배열은 `Map`이라는 자료구조의 일종이다. 따라서, `key` `value`로 이루어진 데이터 형식으로도 사용될 수 있다.

```php
$arr = ['key' => 'value'];

$arr['key']; // value
```

이러한 배열을 `연관배열`이라고 표현한다.
이는 `mysqli_fetch_assoc()` 함수의 결과값으로 리턴되는 배열의 형식이다. 여기서 `assoc`은 `association`이다.

## object

객체는 현실에서 어떤 한 사물(개념)을 표현하는데 사용될 수 있다.

예를 들어, 웹사이트의 회원 한명 한명의 데이터를 객체로 표현해보자.

```php
class Member
{
    private $name;
    private $email;
    private $phoneNumber;
    private $password;

    public function __construct($name, $email, $phoneNumber, $password)
    {
        $this->name         = $name;
        $this->email        = $email;
        $this->phoneNumber  = $phoneNumber;
        $this->password     = $password;
    }
}

$member = new Member('홍길동', 'MrHong@naver.com', '01012341234', 'pw');
```

객체지향 개념을 이용하면, 코드를 깔끔하게 관리할 수 있다.

다음 코드는 php 프레임워크중 하나인 라라벨에서 회원정보를 얻어와서 DB에 저장하는 코드이다.

```php
namespace App\Http\Controllers;

use Illuminate\Http\Request;
use App\User;

class MainController
{
    // 클라이언트에서 회원가입버튼을 누르면, 아래의 메서드가 실행된다.
    public function join(Request $request)
    {
        // 클라이언트가 요청한 데이터는 모두 Request 객체에 들어있다.
        // 그리고 Request객체의 all메서드를 이용해서, 클라이언트가 요청한 POST데이터를 연관배열로 가져올 수 있다.
        $data = $request->all();

        $id = $data['id'];
        $password = $data['password'];
        $email = $data['email'];

        // 새로운 회원정보를 담을 객체를 생성한다.
        $user = new User();

        $user->id = $id;
        $user->password = $password;
        $user->email = $email;

        // User객체의 save메서드를 실행하면, User객체에 저장된 정보를 바탕으로
        // 데이터베이스에 데이터를 입력시킬 쿼리를 자동으로 생성하여 INSERT 쿼리를 날린다.
        $user->save();

        // 회원가입이 완료되었다는 응답을 보낸다.
        return response('회원가입 완료!');
    }
}
```

물론, 입력된 데이터를 바탕으로 자동으로 쿼리를 생성해서 `INSERT`시키는 메서드인 `save()` 등은 `User`클래스에서 미리 구현해야한다.

하지만 이렇게 한번 구현해놓고 나면 실제로 서비스되는 코드는 알아보기가 매우 쉬워진다.

객체는 연관된 데이터를 저장하고, 해당 데이터를 처리하는 메서드들을 정의해놓고 데이터를 쉽게 다룰 수 있게 해준다.

## null

`null`은 데이터가 없음을 나타내는 데이터 타입이다.

---

# 변수

변수는 변하는 수이다.

프로그래머는 변수를 선언하고, 이 선언한 변수에 데이터를 넣을 수 있고, 넣은 데이터를 사용할 수 있다.

프로그래밍을 하다보면 수 많은 데이터가 필요할 것이다. 예를 들어, 학생 30명의 성적 데이터가 있다고 보자. 학생 한명 한명의 점수를 전부 프로그래머가 외워야 할까? 그럴 필요가 없다.

프로그래머는 이해하기 쉬운 단어로된 변수를 선언하고, 이를 이용하면 된다.

```php
$student1 = 100;
$student2 = 90;
// ...
```

각 학생은 본인의 번호가 있으므로, 학생1, 학생2, 학생3 ... 으로 변수이름을 지어놓으면 특정 학생의 점수데이터를 기억할 필요 없이, 맨 처음에 변수를 선언할 때에 데이터를 넣어주고 나중에 해당 변수이름으로 데이터를 사용하면 된다.

물론 위처럼 각 학생마다 변수를 하나씩 만드는건 매우 비효율적이므로 배열을 사용하면 된다.

```php
$students = [100, 90, 80, ...];
```

배열의 인덱스는 0부터 시작하므로, 1번 학생의 경우 $students[0]에 값이 들어있을 것이다. 물론 직관적으로 만들고 싶다면, 인덱스0에 굳이 데이터를 넣지 않고 인덱스1부터 데이터를 넣어도 된다. 이건 프로그래머가 알아서 결정할 일이다.

여튼 중요한점은, 변수는 어쨌든 데이터라는 것이다. 다만 프로그래머가 이름을 지어준 데이터다. 따라서 적절하게 코드 내에서 이 데이터를 사용하면 된다. 

변수 이름을 작명할 때에는, 해당 변수가 가지고 있는 데이터를 잘 설명해주는 단어로 결정하면 된다. 예를 들어, 쿼리를 날리는 쿼리문을 저장하는 변수 이름은 `$query`가 가장 적당할 것이다.



