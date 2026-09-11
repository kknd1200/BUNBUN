# BUNBUN

여행용 한국어 · 베트남어 · 영어 · 일본어 번역기입니다.

- 웹 번역: OpenAI 서버 번역 + 무료 번역 폴백
- 음성 읽기(TTS), 음성 입력(STT)
- 일본어 지원
- PWA 설치 지원
- 브라우저/앱에 OpenAI API 키를 저장하지 않음

## Vercel 배포

Vercel에서 이 GitHub 저장소를 Import한 뒤 프로젝트 이름을 `BUNBUN`으로 설정하세요.

환경 변수:

- `OPENAI_API_KEY` : 필수
- `ACCESS_CODE` : 선택
- `DAILY_LIMIT` : 선택 (기본 2000)

Root Directory는 저장소 최상위(`./`)를 사용하면 됩니다.
