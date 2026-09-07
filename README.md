# buyback-data

삼성전자·SK하이닉스 자사주 매입 실데이터 스냅샷. 매 거래일 저녁 GitHub Actions(`DABINSA/buyback-tracker`)가
한국거래소 KIND 「자사주취득/처분」 신고·신청·체결내역을 그대로 수집해 커밋한다. 커밋 이력이 곧 일별 원천 기록이다.

- `kind.json` — KIND 원천(신고내역: 예정수량·누적취득수량·누적취득금액 / 체결내역: 일별 신청·체결 / 신청내역: 당일 신청·잔여)
- `snapshot.json` — 위 원천 + 네이버(투자자별·종가·코스피) + 다음(환율)로 계산한 당일 스냅샷(남은 수량·속도·예상 소진일)

페이지: https://buyback-tracker-delta.vercel.app
