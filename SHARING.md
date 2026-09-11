# 다른 기기/사람에게 공유하기

이 버전은 OpenAI API 키를 **Vercel 서버에 한 번만** 설정합니다.
휴대폰, 태블릿, PC마다 API 키를 다시 넣을 필요가 없습니다.

```
사용자 기기  ──▶  BUNBUN Vercel 서버  ──▶  OpenAI
 API 키 없음             OPENAI_API_KEY 보관
```

## 필수 설정

Vercel → `BUNBUN` → Settings → Environment Variables

- `OPENAI_API_KEY`: 필수
- `DAILY_LIMIT`: 선택 (기본 2000)
- `ACCESS_CODE`: 선택

`ACCESS_CODE`를 비워두면 앱 주소만 열어도 바로 OpenAI 서버 번역이 됩니다.

## 접속 코드를 켜고 싶을 때

외부 사용으로 인한 비용을 조금 더 통제하려면 `ACCESS_CODE`를 설정할 수 있습니다.
그 경우 아래처럼 공유하면 코드가 자동 입력됩니다.

```
https://<BUNBUN에 할당된 Vercel 도메인>/?code=원하는코드
```

OpenAI API 키 자체는 어떤 경우에도 브라우저로 전달되지 않습니다.

## 비용 보호

현재 서버 함수에는 입력 길이 제한, IP별 호출 제한, 전체 일일 호출 제한이 있습니다.
서버리스 메모리 기반 제한은 완전한 과금 방어가 아니므로 OpenAI/Vercel 쪽 사용량 및 예산 제한도 함께 설정하는 것을 권장합니다.
