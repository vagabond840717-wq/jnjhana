# HANA STAY — 청소 스케줄 앱 (JnJ)

전체 규칙: `vagabond840717-wq/hana-stay` 저장소의 CLAUDE.md 참고.

---

## 이 앱 정보
- **테마**: 다크 `#0f0f0f`
- **배포**: GitHub Pages (이 저장소 루트 index.html)
- **백엔드**: `https://ical-proxy.vagabond1984.workers.dev`

## 핵심 기능
- 체크아웃/체크인 날짜 기반 청소 일정 표시
- 멀티 플랫폼 iCal 파싱 (Airbnb / Booking.com / Trip.com / 리브애니웨어)
- 비밀번호/메모 관리

## 예약 앱(booking)과의 차이
| 기능 | 이 앱 | booking 앱 |
|------|-------|-----------|
| 오버부킹 감지 | ✗ | ✓ |
| 블락 처리 | ✗ | ✓ |
| 달력 스크롤 | 가로만 | 가로+세로 |
| PWA/푸시 | ✗ | ✓ |

## 수정 시 필수 체크
- [ ] 예약 앱(booking)도 같이 수정 필요한지 확인
- [ ] render() 후 attachCellClicks() 체인 유지
- [ ] 월 값 0-indexed 확인 (5 = 6월)

## 작업 원칙
- 큰 기능: 설계 먼저 → 사용자 승인 후 구현
- 승인 없이 다음 단계 진행 금지
- 설명은 코딩 용어 말고 일상 비유로
- 작업 완료 후 hana-stay 저장소의 STATUS.md 업데이트 요청할 것
