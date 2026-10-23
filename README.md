# 토끼 소설 (개인용 Mangayomi 소설 확장)

Mangayomi **Novel extensions repo**에 등록하는 개인용 배포 저장소입니다.

## 등록 주소

```text
https://raw.githubusercontent.com/seekmind1-collab/toki-novel-personal/main/index.min.json
```

Mangayomi의 **Novel extensions repo**에 위 주소를 추가한 뒤 **Novel Extensions**에서 **토끼 소설 (개인)**을 설치하세요. 기존 **토끼 소설** 확장과는 별개 항목입니다.

## 변경 내용

- 기본 도메인: `https://newtoki1.org`
- 주소 직접 지정 옵션을 앱의 `SharedPreferences.get()`에서 읽도록 수정
- 수동 주소를 지정하지 않아도 구형 `toki31~35` 주소로 자동 전환되지 않도록 중앙신호등 조회 비활성화
- 원본의 인기·최신 목록, 검색, 필터, 작품·회차, 본문 처리 로직 유지
- 다른 확장과 충돌하지 않도록 별도 확장 ID 사용

## 주의 사항

- 코드 로직과 주소 처리만 정적/모의 환경에서 검사했습니다. **실제 사이트 응답 또는 Mangayomi 기기에서 목록·본문의 종단 간 성공은 검증되지 않았습니다.**
- 사이트가 요청을 차단하거나 HTML/API가 변경된 경우 추가 수정이 필요할 수 있습니다.
- 썸네일·이벤트 카드 등의 일부 리소스는 원래 배포 서버를 계속 참조합니다.
- 원본 코드 제공자: **wankyo83**, 기존 확장 **토끼 소설 v0.2.7**. 사용자가 제공한 원본 JavaScript를 바탕으로 설정과 기본 도메인만 수정했습니다. **원본 코드의 라이선스와 재배포 허용 여부는 확인되지 않았습니다.** 공개 배포를 지속하기 전에 원저작자의 허락/라이선스를 확인하세요.

## 파일

- `index.min.json` — Mangayomi Novel 저장소 목록
- `javascript/novel/src/ko/toki_novel.js` — 실제 소설 확장 프로그램
