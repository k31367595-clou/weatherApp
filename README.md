# Weatherly

Open-Meteo 데이터를 활용해 현재 날씨와 예보를 한눈에 보여 주는 반응형 날씨 웹앱입니다. 데스크톱에서는 정보를 카드 형태로 좌우에 배치하고, 휴대폰에서는 읽기 쉬운 한 열 화면으로 바뀝니다.

## 주요 기능

- 현재 날씨: 기온, 체감온도, 습도, 바람, 강수량
- 시간별 날씨: 현재부터 24시간의 기온, 날씨 상태, 비 올 확률
- 7일 예보: 최고/최저 기온, 날씨 상태, 비 올 확률
- 도시 변경: 제주, 서울, 부산, 강릉 지원
- 온도 단위 변경: 섭씨(°C)와 화씨(°F) 전환
- 대기질: AQI, PM2.5, PM10 확인
- 반응형 화면: PC·태블릿·모바일 지원

## 사용 기술

- React + TypeScript + Vite
- Lucide React 아이콘
- Open-Meteo Forecast API 및 Air Quality API

## 로컬에서 실행하기

### 1. 저장소 내려받기

```bash
git clone https://github.com/k31367595-clou/weatherApp.git
cd weatherApp
```

### 2. 필요한 패키지 설치

```bash
npm install
```

### 3. 개발 서버 실행

```bash
npm run dev
```

터미널에 표시된 주소(일반적으로 `http://localhost:5173`)를 브라우저에서 열면 앱을 볼 수 있습니다.

## 배포용 빌드 만들기

```bash
npm run build
```

완성된 정적 파일은 `dist` 폴더에 생성됩니다. 로컬에서 배포용 결과물을 확인하려면 아래 명령어를 실행하세요.

```bash
npm run preview
```

## 날씨 데이터 안내

이 앱은 브라우저에서 Open-Meteo API를 호출합니다. 별도의 API 키 없이 예보와 대기질 정보를 가져올 수 있으며, 네트워크 연결이 되지 않을 때에도 화면 구성을 확인할 수 있도록 예시 데이터를 표시합니다.

- [Open-Meteo 날씨 예보 문서](https://open-meteo.com/en/docs)
- [Open-Meteo 대기질 문서](https://open-meteo.com/en/docs/air-quality-api)

## 명령어 모음

| 명령어 | 설명 |
| --- | --- |
| `npm run dev` | 개발 서버 실행 |
| `npm run build` | 타입 검사 및 배포용 파일 생성 |
| `npm run preview` | 배포용 빌드 미리 보기 |
| `npm run lint` | 코드 검사 |
