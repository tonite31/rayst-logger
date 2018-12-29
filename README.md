# rayst-logger
nodejs기반의 서버를 위한 로깅 모듈

이 프로젝트는 분산 서버 구조에서 원인을 빠르게 파악하고 손쉬운 모니터링이 가능한 로깅 시스템을 구축을 목표로 하고 있습니다.

위 목표를 만족하기 위해 다음과 같은 요구사항이 만족되어야 합니다.
1. N대의 서버로그를 1대의 서버로그처럼 볼 수 있어야 한다.
2. 요청-응답 사이의 모든 로그를 시간 순서대로 볼 수 있어야 한다.
3. 에러 발생시 정확한 stack trace를 볼 수 있어야 하며, 요청부터 에러 발생까지의 모든 로그를 볼 수 있어야 한다.
4. 특별한 상황에서만 발생하는 로그를 손쉽게 추적할 수 있어야 한다.
5. 에러 발생시 다양한 방법으로 알림을 줄 수 있어야 한다.

위 요구사항을 만족하기 위해 다음과 같은 기능들이 필요 합니다.
1. 로그 publish를 위한 다양한 adapter 기능.
2. 비동기 처리 등의 상황에도 논리적 흐름을 유지할 수 있는 기능
3. 에러 발생시 notification을 위한 다양한 adapter 기능.
4. 태그 기능

마지막으로 이 프로젝트의 로그를 손쉽게 모니터링하고 검색할 수 있는 서비스가 필요 합니다.
