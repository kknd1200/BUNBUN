# BUNBUN

모바일 여행 통역기 웹앱입니다.

지원 언어: 한국어, 베트남어, 영어, 일본어

## Vercel 환경변수

- `OPENAI_API_KEY` — 필수
- `ACCESS_CODE` — 선택 (기기별 입력을 없애려면 설정하지 않음)
- `DAILY_LIMIT` — 선택 (기본 2000)

브라우저나 APK 안에 OpenAI API 키를 저장하지 않습니다. 프론트엔드는 `/api/translate`만 호출하고 Vercel 서버리스 함수가 OpenAI API를 호출합니다.
