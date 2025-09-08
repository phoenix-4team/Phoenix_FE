# 🔥 재난훈련ON (Phoenix FE)

가상현실과 시뮬레이션을 통해 재난 상황에 대한 대응 능력을 향상시키는 혁신적인 훈련 플랫폼의 프론트엔드 애플리케이션입니다.

## ✨ 주요 기능

- 🎮 **가상현실 훈련**: 실감나는 가상 환경에서 직접 체험하는 재난 대응 훈련
- 🎯 **실시간 시나리오**: 다양한 재난 상황을 실시간으로 시뮬레이션
- 📊 **성과 분석**: 훈련 결과를 체계적으로 분석하고 개선점 제시
- 🔄 **반복 훈련**: 필요한 만큼 반복하여 완벽한 대응 능력 향상
- 👥 **팀워크 훈련**: 여러 명이 함께 참여하여 협력과 소통 능력 향상
- 📱 **모바일 지원**: 언제 어디서나 접근 가능한 반응형 웹 애플리케이션
- 🛡️ **안전 보장**: 실제 위험 없이 안전하게 훈련할 수 있는 환경

## 🛠️ 기술 스택

### Frontend
- **React 19.1.1** - 최신 React 버전으로 구축된 사용자 인터페이스
- **TypeScript** - 타입 안전성을 보장하는 개발 환경
- **Vite** - 빠른 개발 서버와 빌드 도구
- **Tailwind CSS** - 유틸리티 우선 CSS 프레임워크
- **React Router DOM** - 클라이언트 사이드 라우팅
- **React Hook Form** - 효율적인 폼 관리
- **Zustand** - 가벼운 상태 관리 라이브러리
- **TanStack Query** - 서버 상태 관리 및 캐싱
- **Axios** - HTTP 클라이언트

### UI/UX
- **Styled Components** - CSS-in-JS 스타일링
- **React Confetti** - 성취감을 높이는 시각적 효과
- **Custom Animations** - 부드러운 사용자 경험을 위한 애니메이션
- **Dark Mode** - 다크/라이트 테마 지원

## 📁 프로젝트 구조

```
Frontend/
├── public/                 # 정적 파일
│   ├── character.png      # 메인 캐릭터 이미지
│   ├── favicon.png        # 파비콘
│   └── scenarios/         # 시나리오 데이터
├── src/
│   ├── components/        # 재사용 가능한 컴포넌트
│   │   ├── layout/        # 레이아웃 컴포넌트
│   │   ├── ui/           # UI 컴포넌트
│   │   └── ...
│   ├── pages/            # 페이지 컴포넌트
│   │   ├── auth/         # 인증 관련 페이지
│   │   ├── scenario/     # 시나리오 페이지
│   │   └── training/     # 훈련 페이지
│   ├── hooks/            # 커스텀 훅
│   ├── services/         # API 서비스
│   ├── stores/           # 상태 관리
│   ├── types/            # TypeScript 타입 정의
│   └── assets/           # 이미지 및 기타 자산
├── scripts/              # 유틸리티 스크립트
│   ├── scenario-generator/ # 시나리오 생성 도구
│   └── game-script-tool/  # 게임 스크립트 관리 도구
└── ...
```

## 🚀 시작하기

### 필수 요구사항

- Node.js 18.0.0 이상
- npm 또는 yarn

### 설치 및 실행

1. **저장소 클론**
   ```bash
   git clone https://github.com/phoenix-4team/Phoenix_FE.git
   cd Phoenix_FE/Frontend
   ```

2. **의존성 설치**
   ```bash
   npm install
   ```

3. **환경 변수 설정**
   ```bash
   cp env.example .env
   # .env 파일을 편집하여 필요한 환경 변수 설정
   ```

4. **개발 서버 실행**
   ```bash
   npm run dev
   ```

5. **브라우저에서 확인**
   ```
   http://localhost:5173
   ```

## 📜 사용 가능한 스크립트

### 개발
- `npm run dev` - 개발 서버 실행
- `npm run dev:scripts` - 스크립트 도구 개발 서버 실행

### 빌드
- `npm run build` - 프로덕션 빌드
- `npm run build:scripts` - 스크립트 도구 빌드

### 코드 품질
- `npm run lint` - ESLint를 통한 코드 검사

### 미리보기
- `npm run preview` - 빌드된 앱 미리보기
- `npm run preview:scripts` - 스크립트 도구 미리보기

### 시나리오 관리
- `npm run scenario:convert` - 시나리오 변환
- `npm run scenario:convert-all` - 모든 시나리오 변환
- `npm run scenario:validate` - 시나리오 데이터 검증

## 🎨 디자인 시스템

### 색상 팔레트
- **Primary**: 오렌지 계열 (#f97316)
- **Dark Mode**: 다크 그레이 계열
- **Accent**: 빨간색 계열 (재난/긴급 상황 표현)

### 애니메이션
- **Fade In/Out**: 부드러운 등장/퇴장 효과
- **Slide**: 좌우/상하 슬라이드 효과
- **Bounce**: 생동감 있는 바운스 효과
- **Typing**: 타이핑 애니메이션

## 🔧 개발 도구

### 시나리오 생성기
`scripts/scenario-generator/` 디렉토리에는 시나리오 데이터를 생성하고 관리하는 도구가 포함되어 있습니다.

### 게임 스크립트 도구
`scripts/game-script-tool/` 디렉토리에는 게임 스크립트를 관리하는 웹 기반 도구가 포함되어 있습니다.

## 🚀 배포

### Docker를 사용한 배포
```bash
# Docker 이미지 빌드
docker build -t phoenix-fe .

# 컨테이너 실행
docker run -p 80:80 phoenix-fe
```

### AWS Amplify를 사용한 배포
`amplify.yml` 파일이 포함되어 있어 AWS Amplify를 통한 자동 배포가 가능합니다.

## 🤝 기여하기

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 배포됩니다. 자세한 내용은 `LICENSE` 파일을 참조하세요.

## 📞 문의

프로젝트에 대한 문의사항이나 제안사항이 있으시면 이슈를 생성해 주세요.

---

**재난훈련ON**으로 안전한 미래를 만들어가세요! 🔥
