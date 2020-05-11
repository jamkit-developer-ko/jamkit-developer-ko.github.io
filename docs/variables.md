---
layout: page
title: 환경변수와 템플릿 변수
nav_order: 15
---

# {{page.title}}

## 기본 환경변수

모든 sbml/sbss에는 다음 환경변수가 기본으로 지정되어 있다. 

### (1) 실행환경

| 이름 | 값 | 설명 |
|---|---|---|
| OS | Android/iOS | 현재 디바이스의 운영체제 |
| LANGUAGE | 2자리 언어코드| 현재 디바이스의 사용언어 |
| APPID | | 앱 ID |
| HOST_APPID | | 호스트 앱의 ID |
| ORIENTATION | portrait, landscape | 로딩 시의 화면 방향 |
| NETWORK_STATUS | offline, cellular, wifi | 로딩 시의 네트워크 상태 |
| CATALOG_APPID | | 현재 카탈로그의 앱 ID |
| CATALOG_VERSION | | 현재 카탈로그의 버전 |
| LOGGED_IN | yes, no | 북잼 클라우드 로그인 여부 |
| ADULT_STATUS | verified, unknown | 성인 인증 상태 |
| STORE | google, apple, bookjam | 앱내 구매를 위한 기본 스토어 |

### (2) UI 환경

| 이름 | 값 | 설명 |
|---|---|---|
| SUBVIEW | | 현재의 서브뷰 |
| LAYOUT | | 현재의 레이아웃 |
| DISPLAY_UNIT | | 현재의 데이터 ID |

### (3) 현재 시간 

| 이름 | 값 | 설명 |
|---|---|---|
| YEAR | 4자리 숫자 | 로딩 시의 연도 |
| MONTH | 1부터 12사이의 숫자 | 로딩 시의 월 |
| DAY | 1부터 31사이의 숫자 | 로딩 시의 일 |
| HOUR | 0부터 23사이의 숫자 | 로딩 시의 시 |
| MINUTE | 0부터 59사이의 숫자 | 로딩 시의 분 |
| SECOND | 0부터 59사이의 숫자 | 로딩 시의 초 |
| WEEKDAY | SUN, MON, TUE, ..., SAT | 로딩 시의 요일 |
| TIMESTAMP | 숫자 | 로딩 시의 타임스탬프 |

### (4) 멤버십과 포인트 정보

앱에서 사용하는 여러 멤버십과 포인트 각각에 대해 지정된다.

| 이름 | 값 | 설명 |
|---|---|---|
| 멤버십 ID ```M_XXXX_...``` | valid, invalid | 해당 멤버십의 상태 |
| 포인트 ID ```O_XXXX_...``` | activated, inactivated | 해당 포인트의 상태 |
