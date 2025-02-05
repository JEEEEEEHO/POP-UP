### 1. NL

### 2. HASH

[개념]

- ORACLE 이 정한 임계치가 오계 되면 → HASH JOIN을 수행함
- DRIVING TABLE에서 추출한 값을 기준으로 NL 조인이 돌기 때문에 작은 테이블이여야 함
- HASH로 변경된 값들이 NL을 하는 공간은 HASH AREA 라고 함
    
    ![PROBE 테이블에 변환된 HASH 값이 DRIVING TABLE 에 HASH 값과 같은 것을 NL 로 찾음](https://prod-files-secure.s3.us-west-2.amazonaws.com/e10c09c5-4e77-459d-8e69-5bc0f5f89acf/c0c75816-b595-46b1-9bcf-afd00119b1b5/image.png)
    
    PROBE 테이블에 변환된 HASH 값이 DRIVING TABLE 에 HASH 값과 같은 것을 NL 로 찾음
    
    - PGA 세션
    - 총 256개 생성 가능
- 해당 HASH AREA가 메모리에 올라감
    
    (그 메모리를 ***PGA*** 라고 함 = 프로세스에 할당 된 독립된 공간)
    

**[장점]**

- CPU가 수행하는 세션 메모리***PGA*** 에서 수행되기 때문에 빠름

**[단점]**

- 세션 메모리에 만들어진 HASH AREA는 한번 수행 후 없어지기 때문에 재활용이 어려움
    - 따라서 OLTP 와 같이 수행이 자주 일어나는 쿼리는 비효율적 (⇒ 배치에 어울림)
- 다시 한번 옵티마이저가 HASH 값으로 PARSING 해야하는 시간이 필요하기 때문에 자원 소모가 있음
- CPU 사용하기 때문에 과부하 문제가 있을 수 있음