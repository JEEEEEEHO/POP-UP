## 운영체제

<details>
    <summary>
        프로세스와 스레드의 차이를 설명해보세요.250305MON
    </summary>

  <p>
</details>
<details>
    <summary>
        컨텍스트 스위칭에 대해 설명해보세요.250306TUE
    </summary>
        <p>[나의 답변] 프로세스가 진행되면서 스레드에게서 작업을 할당받은 CPU가 스레드 작업을 처리할 때, 스레드를 번갈아가며 처리하게 됨. 이때 하나의 작업을 홀딩하고 다른 작업을 실행함에 앞서서 이전 작업에 대한 작업 내용을 메모리에 저장하는 과정을 말함. 
  </br>
</details>
<details>
    <summary>
        동기와 비동기의 차이(블로킹, 넌블로킹) / 장단점에 대해 설명해보세요.250308SAT
    </summary>
</details>
<br><br>

## 네트워크

<details>
    <summary>
        웹 통신의 큰 흐름: https://www.google.com/ 을 접속할 때 일어나는 일 250305MON
    </summary>
    </br>
    <p>DNS 서버에 url 에 해당하는 서버 ip 번호를 가져옴 
    <p> -> 해당 ip 주소를 가지고 있는 서버로 요청이 전달됨
    <p> -> 서버는 클라이언트가 보낸 http 요청 메세지를 해석
    <p> -> 클라이언트에게 보낼 http 응답 메세지 작성
    </br>
</details>
<details>
    <summary>
        TCP와 UDP의 차이점에 대해서 설명해보세요.250306TUE
    </summary>
    <p>[나의 답변]tcp ip 4계층? 에서 수신 받은 데이터 패킷을 보내는 방법에 차이가 있음.
Tcp 의 경우는 순서까지 함께 패킷 정보에 넘겨서 다음계층? 으로 보내지만
Udp 는 순서는 상관없이 무작위로 패킷을 전송하여 빠른 전송 속도를 보장할 수 있음.
</details>
<details>
    <summary>
        TCP 3, 4 way handshake에 대해서 설명해보세요.250308SAT
    </summary>
</details>
<br><br>

## 언어 - Java

<details>
    <summary>
        JVM의 구조와 Java의 실행방식을 설명해주세요.250305MON
    </summary>

</details>
<details>
    <summary>
        GC가 무엇인지, 필요한 이유는 무엇인지, 동작방식에 대해 설명해주세요.250306TUE
    </summary>
    <p>[나의 답변] Jvm? 내부에 있는 기능으로 힙영역에 저장된 데이터들 중에 사용 종료 생명주기가 다한 것들을 저장하는 공간. 
사용하고 있는 모든 데이터들이 메모리에 저장이 되면 메모리 차지율이 많이 높아지기 때문.
</details>
<details>
    <summary>
        컬렉션 프레임워크에 대해서 설명해주세요.250308SAT
    </summary>
</details>
<br><br>

## 스프링

<details>
    <summary>
        Spring DI/IoC는 어떻게 동작하나요?250305MON
    </summary>
</details>
<details>
    <summary>
        Spring Bean이란 무엇인가요?250306TUE
    </summary>
    <p>[나의 답변] 스프링 컨테이너에 싱글톤 패턴으로 저장되는 객체를 말함.
스프링은 컴포넌트 스캔을 통해 빈에 등록해야할 클래스들을 찾고 이를 컨테이너에 등록함. 해당 클래스들이 호출되면 빈에 등록된 클래스를 반환하게 됨. 
</details>
<details>
    <summary>
        스프링 Bean의 생성 과정을 설명해주세요.250308SAT
    </summary>
</details>
<br><br>

## 데이터베이스

<details>
    <summary>
        데이터베이스에서 인덱스를 사용하는 이유 및 장단점에 대해 설명해주세요.250305MON
    </summary>
</details>
<details>
    <summary>
        트랜잭션에 대해서 설명해주세요.250306TUE
    </summary>
    <p>[나의 답변] 데이터의 변경 조회 등을 수행하는 작업의 단위.
</details>
<details>
    <summary>
        ACID에 대해서 설명해주세요.250308SAT
    </summary>
</details>
<br><br>

## ORM - JPA

<details>
    <summary>
        JPA 영속성 컨텍스트의 이점(5가지)을 설명해주세요.250308SAT
    </summary>
</details>
<br><br>

## Software Engineering

<details>
    <summary>
        접고 펴는 기능
    </summary>
</details>
<br><br>

## Web

<details>
    <summary>
        접고 펴는 기능
    </summary>
</details>
<br><br>

## Cache

<details>
    <summary>
        접고 펴는 기능
    </summary>
</details>
<br><br>

## CLOUD 및 자료구조

<details>
    <summary>
        배열과 링크드 리스트의 차이를 설명해주세요.250306TUE
    </summary>
    <p>[나의 답변]  배열은 생성될 때부터 길이가 지정이 되고, 배열의 값은 인덱스를 갖기 때문에 그 인덱스로 값을 찾을 수 있음.
추가를 하면 가장 마지막에 가서 저장이 되며 삭제를 하는 경우 뒤에 있는 값들이 앞으로 당겨져서 저장이 됨.

<p>링크드 리스트는 배열과 다르게 생성될 때 부터 길이를 지정할 필요가 없고, 각 인자가 바로 그 이전 이후의 인자 값의 위치를 저장하고 있음. 따라서 데이터를 수정하는 경우 그 앞과 그 후의 위치만 변경하면 되기 때문에 수정을 줄때 성능이 좋음.
? 인덱스는 어디에 저장되지? Get 으로 찾을때는?

</details>

<br><br>

## CI/CD 및 보안

<details>
    <summary>
        비대칭키 암호화, 대칭키 암호화에 대해 간단히 설명해주세요.250306TUE
    </summary>
</details>
<br><br>
