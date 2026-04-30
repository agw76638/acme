| 항목 | 내용 |

| --- | --- |

| **대상 URL** | https://estbootcamp.co.kr |

| **페이지** | 이스트캠프 \| 프론트엔드 14기 |

| **검사 도구** | W3C HTML Validator |

| **요약** | 오류: 약 80건, 경고: 3건, 정보: 다수 |

오류 (Error)

| 번호 | 오류 내용 | 위치 | 수정 방법 |

| --- | --- | --- | --- |

| 1 | 중복 <meta charset> 선언 | line 83 | 첫 번째 선언만 유지하고 두 번째 선언 제거 |

| 2 | <p> 요소를 헤딩 태그 내부에 사용 | h1, h2, h3, h5, h6 | <p>를 헤딩 태그 외부로 이동 |

| 3 | <ul> 요소를 <h6> 내부에 사용 | line 1059, 1125, 1196 | <ul>을 헤딩 태그 외부로 이동 |

| 4 | <iframe> width/height에 퍼센트(%) 값 사용 | line 167~185 | 속성 값을 제거하고 CSS로 대체 |

| 5 | <iframe>에 frameborder 속성 사용 | line 167 | 속성을 제거하고 CSS border: none; 적용 |

| 6 | <button>에 비표준 속성 사용 | line 231~237 | 해당 속성을 제거하고 CSS로 대체 |

| 7 | <img> 요소에 alt 속성 누락 | line 458, 507, 641 등 | 의미 있는 이미지에 alt 추가 |

| 8 | <a> 요소에 href 속성 누락 | line 3104, 3139 | 적절한 href 값 추가 |

| 9 | <a> 내부에 <button> 사용 | line 3105, 3140 | <button> 제거 후 <a> 스타일링 |

| 10 | 잘못된 href URL 형식 | line 3197 | https:// 제거 |

| 11 | 중복 ID | line 115, 3240 | 두 번째 요소의 ID 변경 |

| 12 | <ul> 내부에 <div> 사용 | line 3259, 3282 | <div>를 <li> 내부로 이동 |

| 13 | role="tab" 요소에 대응하는 role="tabpanel" 누락 | line 2005~2011 | tabpanel 요소와 aria-controls 속성 추가 |

| 14 | 헤딩 레벨 순서 건너뜀 | 다수 | 헤딩 레벨을 순차적으로 사용 |

경고 (Warning)

| 번호 | 경고 내용 | 위치 | 수정 방법 |

| --- | --- | --- | --- |

| 1 | <html> 태그에 lang 속성 누락 | line 1~2 | <html lang="ko"> 추가 |

| 2 | viewport 메타에서 사용자 확대/축소 제한 | line 48~51 | maximum-scale 및 user-scalable=no 제거 |

| 3 | frameborder 속성 폐기 | line 167 | CSS로 border: none; 적용 |

정보 (Info)

| 번호 | 정보 내용 | 위치 |

| --- | --- | --- |

| 1 | void 요소의 닫는 슬래시 (/) | 문서 전체 다수 |

우선순위별 수정 권고

| 우선순위 | 항목 | 이유 |

| --- | --- | --- |

| 🔴 즉시 | alt 속성 누락 이미지 | 접근성 법적 요건 (WCAG 2.1) |

| 🔴 즉시 | href 누락 <a> 요소 | 기능 오류 |

| 🔴 즉시 | 잘못된 mailto URL | 이메일 링크 불동작 |

| 🔴 즉시 | 중복 ID | JavaScript/CSS 동작 오류 가능 |

| 🟠 높음 | <p>를 헤딩 내부에 사용 | 구조적 오류, SEO/접근성 저해 |

| 🟠 높음 | <button> inside <a> | 유효하지 않은 HTML 구조 |

| 🟠 높음 | 헤딩 레벨 건너뜀 | 스크린리더 탐색 오류 |

| 🟡 보통 | lang 속성 누락 | 언어 인식 오류 |

| 🟡 보통 | 사용자 확대 차단 viewport | 접근성 저해 |

| 🟡 보통 | <iframe> width/height % | 유효하지 않은 속성값 |

| 🟡 보통 | 비표준 button 속성 | 불필요한 마크업 오염 |

| 🔵 낮음 | frameborder 폐기 속성 | 동작에 영향 없으나 정리 권장 |

| 🔵 낮음 | void 요소 닫는 슬래시 | 동작 영향 없음 |

본 보고서는 W3C HTML Validation 결과를 기반으로 작성되었습니다.
