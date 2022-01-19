# javastudy
  - 2021-08-20
  - 자료형 크기
    - 정수형 
      -  byte (1바이트)
      -  short (2바이트)
      -  int (4바이트)
      -  long (8바이트)
    - 실수형
      - float (4바이트)
      - double (8바이트)
    - 논리형
      - boolean (1바이트)

  - 2021-09-13
  - 매개변수
      - src
        - 복사할 배열 이름
      - srcPos
        - 복사할 배열의 첫 번째 위치
      - dest
        - 복사해서 붙여 넣을 대상 배열 이름
      - destPos
        - 복사해서 대상 배열에 붙여 넣기를 시작할 첫 번째 위치
      - length
        - src에서 dest로 자료를 복사할 수 있습니다.
  - 2021-09-15
  - ArrayList 클래스의 주요 메서드
      - boolean add(E e)
        - 요소 하나를 배열에 추가합니다. E는 요소의 자로형을 의미합니다.
      - int size()
        - 배열에 추가된 요소 전체 개수를 반환합니다.
      - E get(int index)
        - 배열의 index 위치에 있는 요소 값을 제거하고 그 값을 반환합니다.
      - E remove(int index)
        - 배열의 index 위치에 있는 요소 값을 제거하고 그 값을 반환합니다.
      - boolean isEmpty()
        - 배열이 비어 있는지 확인합니다.
      - 추상 메서드
        - 예: getNextCall();
  - 2021-10-13
  - 애노테이션
      - @Override
        - 재정의된 메서드라는 정보 제공
      - @Fuctionallnterface
        - 함수형 인처페이스라는 정보 제공
      - @Deprecated
        - 이후 버전에서 사용되지 않을 수 있는 변수, 메서드에 사용됨
      - @SuppressWarnings
        - 특정 경고가 나타나지 않도록 함
  - 2021-10-27
  - 예약어
      - abstract
  - 구현된 메서드
      - 하위 클래스에서 공통으로 사용할 구현 코드, 하위 클래스에서 재정의할 수도 있음
  - 추상 메서드
      - 하위 클래스가 어떤 클래스냐에 따라 구현 코드가 달라짐  
  - 2021-11-01
  - final 예약어
      - 변수
        - final 변수는 상수를 의미합니다.
      - 메서드
        - final 메서드는 하위 클래스에서 재정의할 수 없습니다.
      - 클래스
        - final 클래스는 상속할 수 없습니다. 
  - 접근 제어자                  public    protected    default    private
      같은 패키지, 같은 클래스    허용       허용         허용       허용             
      같은 패키지, 상속 관계      허용       허용         허용       불용
      같은 패키지, 상속 관계 아님  허용      허용         허용       불용
      다른 패키지, 상속 관계      허용       허용         불용       불용
      다른 패키지, 상속 관계 아님  허용      불용         불용       불용
  - 2021-11-07
  - instance
      - 객체 지향 프로그래밍(OOP)에서, 어떤 등급에 속하는 각 객체를 인스턴스라고 함
  - static
      - 공통된 
      - 클래스에선 만들어지기기 전인 인스턴스에 접근 할수 없음.
      - 인스턴스에선 부모격인 클래스에 접근할 수 있음.
      - 공유폴더의 내용물. 안의 내용물을 볼 수 있고, 사용할 수 있지만, 폴더의 내용물을 수정하면 해당 폴더를 공유하고 있는 모든 사용자에게도 수정된 결과물이 보여짐
      - 1. static이 있는 건 클래스 소속, static이 없는 건 인스턴스 소속
      - 2. 클래스로 정의된 변수나 메소드는 클래스를 통해서 접근 가능하지만 인스턴스로 정의된 변수나 메소드는 해당 클래스의 인스턴스를 생성해야만 접근할 수 있다.
      - 3. 인스턴스에서 해당 클래스로 정의된 변수를 수정하면 그 클래스를 포함한 모든 인스턴스의 변수가 
수정되지만, 인스턴스에서 해당 인스턴스로 정의된 변수를 수정하면 해당 인스턴스의 변수만 수정된다.
  - 2021-11-08
  - 인터페이스
      - 큰 틀   
      - 클래스 혹은 프로그램이 제공하는 기능을 명시적으로 선언하는 역할을 한다. 
      - 추상 메서드와 상수로만 이루어져 있다.
      - 구현된 코드가 없을 때 당연히 인터페이스를 생성할 수 없다.
      - 디폴트 메서드와 정적 메서드 구현부가 없다면 인터페이스는 껍데기가 된다.
  - 인터페이스의 역할
      - 서버와 대응돼는 프로그램에서 어떤 메서드를 제공하는지 미리 알려주는 명세 또는 약속의 역할을 한다. 
      - 인터페이스를 구현한 클래스가 어떤 기능의 메서드를 제공하는지 명시하는 것이다.
      - 클라이언트 프로그램은 인터페이스에서 약속한 명세대로 구현한 클래스를 생성해서 사용하면 됌.
  - 인터페이스와 다형성 
      - 인터페이스를 사용하면 다형성을 구현하여 확장성 있는 프로그램을 만들 수 있다.
      - 클라이언트 프로그램을 많이 수정하지 않고 기능을 추가하거나 다른 기능을 사용할 수 있다.
  - 상속 
      - extends 
        - 부모에서 선언/정의를 모두하며 자식은 메소드/변수를 그대로 사용할 수 있음
        - extends가 상속의 대표적인 형태                                              
        - 부모의 메소드를 그래도 사용할 수 있으며 오버라이딩 할 필요 없이 부모에 구현 되있는 것을 직접 사용 가능
      - implements 
        - 부모 객체는 선언만 하며 정의(내용)은 자식에서 오버라이딩(재정의)해서 사용해야함
      - abstract
        - extends와 interface 혼합. extends하되 몇 개는 추상 메서드로 구현되어 있음
      - 클래스일때
        - 클래스 내에 추상메서드가 선언되어 있음을 의미
      - 메서드일때
        - 선언부만 작성하고 구현부는 작성하지 않는 추상메서드임을 알림
      - 정리
        - extends는 일반 클래스와 abstract 클래스 상속에 사용되고, implement는 interface 상속에 사용
        - class가 class를 상속받을 땐 extends를 사용하고, interface가 interface를 상속 받을 땐 extends를 사용
        - class가 interface를 사용할 땐 implements를 써야함
        - interface가 class를 사용할 땐 implements를 쓸수 없음
        - extends는 클래스 한 개만 상속 받을 수 있음
        - extends 자신 클래스는 부모 클래스의 기능을 사용
        - implements는 여러개 사용 가능
        - implements는 설계 목적으로 구현 가능
        - implements한 클래스는 implements의 내용을 다 사용해야 함
  - 2021-11-15
  - 오버라이딩
     - 조상 클래스로부터 상속받은 메서드의 내용을 변경하는 것
  - 오버로딩
     - 기존에 없던 새로운 메서드를 정의하는 것
  - 메서드/생성자
     - Vector()
        - 10개의 객체를 저장할 수 있는 Vector인스턴스를 생성한다. 10개 이상의 인스턴스가 저장되면, 자동적으로 크기가 증가
     - boolean add(Object o)
        - Vector에 객체를 추가한다. 추가에 성공하면 결과값으로 true, 실패하면 false를 반환
     - boolean remove(Object o)
        - Vector에 저장되어 있는 객체를 제거한다. 제거에 성공하면 true, 실패하면 false를 반환
     - boolean isEmpty()
        - Vector가 비어있는지 검사한다. 비어있으면 true, 비어있지 않으면 false를 반환
     - Object get(int index)
        - 지정된 위치(index)의 객체를 반환한다. 반환타임이 Object타임이므로 적절한 타임으로의 형변환이 필요
     - int size()
        - Vector에 저장된 객체를 개수를 반환
  - 2021-11-17
  - 참조 자료형
     - 크기가 정해진 기본 자료형으로 선언하는 변수가 있고, 클래스 자료형으로 선언하는 참조 자료형 변수가 있음
  - 정보 은닉
     - 클래스 내부에서 사용할 변수나 메서드는 private으로 선언해서 외부에서 접근하지 못하도록 하는 것을 객체 지향에서 정보 은닉이라 함!
     - 접근 제어자를 private로 선언한 변수는 같은 클래스에서만 가능하고 외부클래스에서는 get, set을 사용해야 한다.
  - 접근 제어자
     - public
        - 외부 클래스 어디에서나 접근할 수 있다.
     - protected
        - 같은 패키지 내부와 상속 관계의 클래스에서만 접근할 수 있고 그 외 클래스에서는 접근할 수 없음.
     - 아무것도 없는 경우
        - default이며 같은 패키지 내부에섬나 접근할 수 있다.
     - private
        - 같은 클래스 내부에서만 접근할 수 있음.
  - this
     - 1) 간단히 설명하면 생성된 인스턴스 스스로를 가리키는 예약어이다.
     - 2)  클래스에 생성자가 여러 개 있을 때 어떤 생성자에서 다른 생성자를 호출하는 경우가 종종있다. 이때 this를 사용해 클래스의 생성자에서 다른 생성자를 호출할 수 있다.
     - 3) this를 사용하여 생성된 클래스 자신의 주소 값을 반환할 수 있다. 인스턴스 주소 값을 반환할 때는 this를 사용하고 반환형은 클래스 자료형을 사용한다.
  - 2021-11-24
  - Scanner클래스
     - Scanner 객체 생성
        - Scanner 객체명 = new Scanner(System.in);
          - 객체명도 변수명과 마찬가지로 개발자 마음이다. 
          - import java.util.Scanner; 를 추가해줘야한다.
     - System.in
        - 키보드에서 사용자로부터 키 입력을 받기 위해서는 System.in을 사용한다.
        - 지금은 키보드에서 입력을 받는다는 뜻으로 사용한다고 알아둔다.
     - import문 사용
       - import java.util.Scanner;
        - 자바에서 개발자들을 위해 많은 라이브러리를 제공하는데, 사용하기 위해서 어디에 위치한 것을 사용할 것인지 알려줘야 한다.
        - import문은 Scanner 클래스의 정확한 경로가 java.util.Scanner라고 알려주는 것이다.
  - 2021-12-01
  - 인터페이스 상속하기
     - 인터페이스 간에도 상속이 가능
     - 인터페이스 간 상속은 구현 코드를 통해 기능을 상속하는 것이 아니므로 형 상속이라고 한다.
     - 클래스의 경우에는 하나의 클래스만 상속받을 수 있지만, 인터페이스는 여러 개를 동시에 상속받을 수 있다.
     - 한 인터페이스가 여러 인터페이스를 상속받으면, 상소받은 인터페이스는 상위 인터페이스에 선언한 추상 메서드를 모두 가지게 된다.
  - 모든 클래스
     - String toString()
        - 객체를 문자열로 표현해서 반환한다.
        - 재정의하여 객체에 대한 설명이나 특정 멤버 변수 값을 반환한다.
     - boolean equals(Object obj)
        - 원래 기능은 두 인스턴스의 주소를 비교하는 것이다.
        - 따라서 같은 주소에만 true가 된다.
        - 두 인스턴스가 동일한지 여부를 반환한다.
        - 재정의하여 논리적으로 동일한 인스턴스임을 정의할 수 있다.
     - int hashCode()
        - 정보를 저장하거나 검색할 때 사용하는 자료 구조이다.
        - 정보를 어디에 저장할 것인지, 어디서 가져올 것인지 해시 함수를 사용하여 구현한다.
        - 객체의 해시 코드 값을 반환한다.
     - Object clone()
        - 객체를 복제하여 동일한 맴버 변수 값을 가진 새로운 인스턴스를 생성한다.
     - Class getClass()
        - 객체의 class클래스를 반환한다.
     - void wait()
        - 멀티스레드 프로그램에서 사용하는 메서드 이다.
        - 스레드를 '기다리는 상태'로 만든다.
     - void finalize()
        - 인스턴스가 힙 메모리에서 제거될 때 가비지 컬렉터(GC)에 의해 호출되는 메서드이다.
        - 네트워크 연결 해제, 열려 있는 파일 스트림 해제 등을 구현한다.
     - void notify()
        - wait()메서드에 의해 기다리고 있는 스레드(non runnable상태)를 실행 가능한 상태(runnable)로 가져온다.
  - 2022-01-07
  - instanceof
     - 비교 연산자로 >, <, ==와 같이 두개의 인재를 받는 연산자로 앞의 비교 연산자들을 이용하는 기분으로 사용하면 된다.
     - instanceof는 클래스의 타입을 감지하는 역할을 하고, 위의 예를 통해 모든 클래스는 기본 클래스인 Object를 확장한다는 것을 알 수 있다.
     - instanceof 연산자는 객체를 어떤 클래스인지, 어떤 클래스를 상속받았는지 확인하는 데 사용하는 연산자이다.
  - 추상클래스
     - 객체를 직접 생성할 수 있는 클래스를 실체클래스라고 한다면, 이 클래스들의 공톨 특성을 추출해서 선언한 클래스 = 추상클래스
     - 추상클래스가 부모, 실제클래스가 자식 실제클래스의 모든 걸 상속받을 수 있음
  - final 예약어
     - final 변수: 상수 변수(값이 변경될 수 없음)
     - final 메서드: 하위 클래스에서 재정의 할 수 없는 메서드
     - final 클래스: 상속할 수 없는 클래스
  - abstract
     - 추상클래스를 만들려면 abstract를 클래스 앞에 붙인다.
#raspberrypi
  2022-1-19
  
  -from bs4 import BeautifulSoup
from urllib.request import Request, urlopen
from urllib.parse import urlencode, quote_plus, unquote
import requests

url = 'http://apis.data.go.kr/B552584/ArpltnInforInqireSvc/getMsrstnAcctoRltmMesureDnsty'
queryParams = '?' + urlencode({quote_plus('serviceKey'): 'Gkhq+uo4qB8ETdZCYbYJHIswWquBvkKR0PKmUHppucbBJztsGx17tq9cx56sDqItq3Ltd8wlQay9PP6yoyUmDQ=='
	,quote_plus('returnType'):'xml'
	,quote_plus('numOfRows'):'10'
	,quote_plus('pageNo'): '1'
	,quote_plus('stationName'): '서창'
	,quote_plus('dataTerm'): 'DAILY'
	,quote_plus('ver'): '1.0'})
	
res = requests.get(url+queryParams)
soup = BeautifulSoup(res.content, 'html.parser')
data = soup.find_all('item')
print(data)	

for item in data:
	datatime = item.find('datatime')
	pm25value = item.find('pm10value')
	print(datatime.get_text())
	print(pm25value.get_text())
	
  -에어코리아 주소
     - airkorea.or.kr
  - 공공데이터 포털 주소
     - data.go.kr   
     - 
