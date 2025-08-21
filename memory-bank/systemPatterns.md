# 시스템 패턴 (System Patterns)

## 아키텍처 개요
- **패턴**: Next.js App Router 기반 아키텍처
- **라우팅**: 파일 시스템 기반 라우팅
- **렌더링**: SSR + CSR 하이브리드

## 디자인 패턴

### 컴포넌트 구조
- **함수형 컴포넌트**: React 19 기능 활용
- **타입 안전성**: TypeScript 인터페이스 활용
- **재사용성**: 컴포넌트 분리 및 추상화

### 스타일링 패턴
- **Utility-First**: Tailwind CSS 접근법
- **반응형 디자인**: 모바일 우선 접근
- **컴포넌트 스타일링**: CSS-in-JS 또는 CSS 모듈

### 상태 관리
- **로컬 상태**: React useState/useReducer
- **서버 상태**: Next.js 내장 데이터 페칭
- **전역 상태**: Context API (필요시)

## 폴더 구조 규칙
```
app/
├── (routes)/           # 라우트 그룹
├── components/         # 재사용 컴포넌트
├── lib/               # 유틸리티 함수
├── types/             # TypeScript 타입 정의
└── styles/            # 스타일 파일
```

## 코딩 컨벤션
- **네이밍**: camelCase (변수/함수), PascalCase (컴포넌트)
- **파일명**: kebab-case 또는 PascalCase
- **Import 순서**: 외부 라이브러리 → 내부 모듈 → 상대 경로

## 성능 패턴
- **코드 분할**: 동적 import 활용
- **이미지 최적화**: next/image 컴포넌트
- **메타데이터**: next/head 또는 metadata API
- **캐싱**: Next.js 내장 캐싱 전략
