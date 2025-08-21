# 기술 컨텍스트 (Technical Context)

## 기술 스택

### 프론트엔드
- **Next.js**: 15.5.0 (App Router)
- **React**: 19.1.0
- **TypeScript**: ^5
- **Tailwind CSS**: ^4

### 개발 도구
- **패키지 매니저**: pnpm (프로젝트 기본 설정)
- **번들러**: Turbopack (Next.js 내장)
- **린터**: ESLint 9 + eslint-config-next
- **타입 체킹**: TypeScript

### 빌드 및 배포
- **개발 서버**: `next dev --turbopack`
- **빌드**: `next build --turbopack`
- **프로덕션**: `next start`

## 프로젝트 구조
```
hello-nextjs/
├── app/                 # App Router 기반 페이지
│   ├── globals.css     # 전역 스타일
│   ├── layout.tsx      # 루트 레이아웃
│   └── page.tsx        # 홈 페이지
├── public/             # 정적 자산
├── docs/               # 프로젝트 문서화
└── 설정 파일들
```

## 개발 환경 설정
- Node.js 환경
- pnpm 패키지 매니저 사용
- ESLint 규칙 적용
- TypeScript 엄격 모드

## 성능 최적화
- Turbopack 번들러 활용
- Next.js 이미지 최적화
- 폰트 최적화 (Geist 폰트)
- 자동 코드 분할
