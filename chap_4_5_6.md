# 대규모 4, 5, 6장 + 디자인패턴

발표자: 우철 양, 완희 남
생성 일시: 2023년 5월 9일 오후 11:03
태그: 질문

> 박은정 - 대규모 2편 : 1장 발표, 2장 읽기

- 인용구
  실제 질문
  ***
  이름태그 : 생각하는 대답

완료

### 4장. 처리율 제한 장치의 설계 @우철 양

- p.55 MSA의 경우 처리율 제한 장치는 보통 API 게이트웨이라 불리는 컴포넌트에 구현된다. API 게이트웨이는 처리율 제한, SSL 종단, 사용자 인증, IP 허용 목록 관리 등을 지원하는 완전 위탁관리형 서비스이다.
  **`MSA 구조 + API 게이트 웨이 역할 더 자세히?`**
  ***
- p.61 이 알고리즘의 가장큰 문제는…
  이해가 되지 않습니다.. 설명 부탁드립니다
  ***
  @박은정 자문자답
  ⇒ 당연하게 문제임. 왜 → 처리율 제한 장치니
  @김윤우
  분당 최대 5개의 요청으로 제한하고 싶어서 고정윈도우를 쓰는 건데, 2:00:30 ~ 2:01:30 까지의 1분을 보면 10개임. 어느 지점부터의 1분이든지 최대 5개로 하고싶다면 이 10개는 허용 한도의 2배가 되어버린다~ 라고 이해했습니당

**`ex0 깜짝 세일 -⇒ 토큰 버킷 적절`**

### 5장. 안정 해시 설계 @완희 남

- Discord 예시 블로그 해석 & 설명 부탁드립니다.
  [How Discord Scaled Elixir to 5,000,000 Concurrent Users](https://discord.com/blog/how-discord-scaled-elixir-to-5-000-000-concurrent-users)

### 6장 @김윤우

[[대규모 시스템 설계 기초] 6장. 키-값 저장소 설계](https://velog.io/@kyy00n/대규모-시스템-설계-기초-6장.-키-값-저장소-설계)

[6장 정리 노트](notes/6%E1%84%8C%E1%85%A1%E1%86%BC%20%E1%84%8C%E1%85%A5%E1%86%BC%E1%84%85%E1%85%B5%20%E1%84%82%E1%85%A9%E1%84%90%E1%85%B3%20adbfe6682f0042a99c74d7c6ea0d1b4d.md)

- p.113 블룸 필터(Bloom Filter) 가 흔히 사용된다.
  블룸 필터가 무엇인가요?
  ***
  [BloomFilter를 이용해서 데이터 찾기.](https://yujuwon.tistory.com/entry/BloomFilter를-이용해서-데이터-찾기)

### 디자인패턴 : (가볍게) 싱글톤 패턴

- 문제점

[Interview_Question_for_Beginner/README.md at master · JaeYeopHan/Interview_Question_for_Beginner](https://github.com/JaeYeopHan/Interview_Question_for_Beginner/blob/master/DesignPattern/README.md)
