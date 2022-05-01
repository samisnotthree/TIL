바이트코드 조작
====================

### 프로그램 분석
- 코드에서 버그 찾는 툴
- 코드 복잡도 계산

### 클래스 파일 생성
- 프록시
- 특정 API 호출 접근 제한
- 스칼라 같은 언어의 컴파일러

### 그밖에도 자바 소스 코드 건리지 않고 코드 변경이 필요한 여러 경우에 사용할 수 있다.
- 프로파일러 (newrelic)
- 최적화
- 로깅
- ...

### 스프링이 컴포넌트 스캔을 하는 방법 (asm)
- 컴포넌트 스캔으로 빈으로 등록할 후보 클래스 정보를 찾는데 사용
- ClassPathScanningCandidateComponentProvider -> SimpleMetadataReader
- ClassReader와 Visitor 사용해서 클래스에 있는 메타 정보를 읽어온다.
