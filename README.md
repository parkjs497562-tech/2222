# 프롬프트 및 후가공 작업 로그

본 문서는 프로젝트 시안 이미지를 생성하고 후가공하는 과정 전반을 추적하기 위한 **실무 작업 로그**입니다.

평가자가 프롬프트의 체계적인 개선 과정과 AI 이미지의 기술적 보정 능력을 한눈에 평가할 수 있도록 단계별로 구성하였습니다.

---

# 1. 생성 화면 기획 및 규격 정의

| 화면 번호 | 화면명 | 화면 핵심 비주얼 요소 | 화면 비율 |
|-----------|---------|----------------------|-----------|
| 01 | 메인 페이지 | 아늑한 우드 톤의 Full-Width 히어로 배너와 투명 오버레이 헤더를 배치하고, 하단에는 이달의 추천 원두 4종과 Best Sellers 상품을 배치 | 16:9 |
| 02 | 상품 상세 페이지 | 좌측 대형 상품 이미지와 우측 상품 정보를 배치한 2단 레이아웃, 산미/바디감 게이지, 플레이버 태그, 하단 고정 Add to Cart 버튼 | 16:9 |
| 03 | 상품 목록 페이지 | 화이트 내비게이션 바, 카테고리 필터, 좌측 필터 사이드바, 상품 카드 Grid Layout 및 Quick Add to Cart 버튼 | 16:9 |

---

# 2. 프롬프트 최적화 이력

기획한 의도가 프롬프트를 거쳐 최종 디자인 이미지로 나타나기까지의 개선 과정을 기록하였다.

---

# v1 (초안)

## 사용 프롬프트

- 메인 페이지
- 상품 목록 페이지
- 상품 상세 페이지

초기 버전에서는 커피 쇼핑몰 UI를 생성하기 위한 기본적인 구조만 포함하였다.

### 한계점

- 브랜드명이 없어 브랜드 정체성이 부족함
- 메인 히어로 상품이 명확하지 않음
- CTA 버튼이 하나뿐이라 프로토타입 연결성이 부족함
- 상품 패키지의 방향이 서로 달라 시각적 통일성이 떨어짐

### 개선 의도

- 브랜드명을 **Home Barista**로 통일
- 투명 Navigation과 Hero Banner를 구체적으로 명시
- Shop Now / View All Products의 역할을 구분
- 모든 상품 이미지를 동일한 방향으로 생성하도록 지시

---

# v2 (개선)

## 프로젝트 개요

### 프로젝트명

**Home Barista**

### 프로젝트 주제

프리미엄 홈카페 원두 쇼핑몰 (Desktop Web)

### 프로젝트 목적

AI 이미지 생성 도구를 활용하여 프리미엄 홈카페 브랜드 콘셉트의 고품질 쇼핑몰 UI를 제작한다.

사용자가 자연스럽게 상품을 탐색하고 구매할 수 있도록 메인, 상품목록, 상품상세의 3개 핵심 화면을 구성하였다.

---

## 사용자 흐름

```text
Home
 ↓
Product Listing
 ↓
Product Detail
```

---

## 타겟 사용자

- 20~40대 홈카페 사용자
- 스페셜티 커피 관심 고객
- 프리미엄 쇼핑 경험을 선호하는 사용자

---

# 프로젝트 컨셉

## 브랜드

> Home Barista

## 브랜드 무드

- Luxury
- Cozy Cafe
- Warm
- Minimal
- Modern

---

## 핵심 키워드

```text
Premium
Specialty Coffee
Home Cafe
Luxury
Warm
Minimal
Modern
High-End Brand
```

---

# 공통 디자인 가이드

## 브랜드명

```text
Home Barista
```

모든 화면에서 동일한 브랜드명을 사용하였다.

---

## Color Palette

```text
Espresso Brown
Cream Beige
Warm White
Soft Gold Accent
```

---

## UI Style

```text
High Fidelity UI
Luxury E-commerce
Modern Desktop Website
Warm Minimalism
Elegant Typography
Rounded Components
Soft Shadows
Premium User Experience
```

---

## Navigation 규칙

- 메인 : Transparent Navigation
- 목록 : White Navigation
- 상세 : White Navigation

모든 화면에서

- 동일한 로고
- 동일한 메뉴
- 동일한 아이콘 위치

를 유지하도록 프롬프트를 구성하였다.

---

## 화면 비율

```text
Desktop Web
16:9 Aspect Ratio
```

---

# 공통 키워드

모든 프롬프트 마지막에 다음 키워드를 추가하였다.

```text
High Fidelity UI
Premium Specialty Coffee Brand
Brand Name: Home Barista
Luxury E-commerce Design
Warm Minimalism
Realistic Product Photography
Consistent Design System
Balanced Layout
Rounded Components
Figma Style
16:9 Aspect Ratio
```

---

# 공통 네거티브 프롬프트

```text
Avoid

blurry image
low quality
mobile layout
cropped elements
duplicate products
watermark
broken typography
anime style
cartoon illustration
messy composition
poor visual hierarchy
pixelated image
```
# 3. 팀원 피드백 검토 및 반영 내역

프로젝트 진행 중 팀원들의 피드백을 수집하였으며, 프롬프트를 통해 반영 가능한 사항을 검토하고 수정하였다.

---

## 1. 브랜드명 통일

### 변경 전

```text
Design a high-fidelity desktop homepage UI for a premium specialty coffee bean e-commerce website.
```

### 변경 후

```text
Design a high-fidelity desktop homepage UI for a premium specialty coffee bean e-commerce website called "Home Barista".
```

### 반영 이유

- 브랜드 아이덴티티 강화
- 모든 화면과 제품 패키지에서 동일한 브랜드 경험 제공

---

## 2. 상단 Navigation 통일

### 변경 전

```text
Include a modern top navigation bar.
```

### 변경 후

```text
Use a consistent navigation design across all pages.

Homepage:
Transparent navigation overlaying the hero image.

Listing Page:
White navigation background.

Detail Page:
White navigation background.
```

### 반영 이유

- 화면 간 통일성 확보
- 하나의 서비스처럼 인식되도록 개선

---

## 3. CTA 버튼 역할 구분

### 변경 전

```text
Add a primary "Shop Now" button.
```

### 변경 후

```text
Include a primary "Shop Now" button for the featured product.

Include a secondary "View All Products" button for browsing the complete coffee collection.
```

### 반영 이유

- 프로토타입 구현 시 버튼 목적을 명확하게 전달하기 위함

---

## 4. 메인 배너 상품 명확화

### 변경 전

```text
Include a full-width hero banner displaying espresso and coffee beans.
```

### 변경 후

```text
Create a hero banner showcasing a signature Home Barista coffee bean product together with espresso and roasted coffee beans.
```

### 반영 이유

- 대표 상품을 명확히 설정하여 Shop Now 버튼과 연결하기 위함

---

## 5. 상품 이미지 방향 통일

### 변경 전

```text
Display four premium coffee bean product cards.
```

### 변경 후

```text
Display four premium coffee bean product cards.

All product package images should face the same direction for visual consistency.
```

### 반영 이유

- 상품 카드 간 시각적 균형 향상
- 브랜드 일관성 강화

---

## 6. 상품 목록과 상품 상세 연결

### 변경 전

```text
Display a modern product grid with 8 premium coffee bean products.
```

### 변경 후

```text
Display a modern product grid with 8 premium coffee bean products.

The first product card should feature the same coffee bean product used in the product detail page.
```

### 반영 이유

- 사용자 쇼핑 흐름 연결
- 프로토타입 자연스러운 이동 구현

---

## 7. 상세 페이지 썸네일 제거

### 변경 전

```text
The main section should display a large premium coffee bean package image.
```

### 변경 후

```text
The main section should display a single large premium coffee bean package image.

Avoid additional thumbnail galleries.
```

### 반영 이유

- 주요 상품 정보에 집중하도록 구성

---

## 8. 상세 페이지 정보 구조 단순화

### 변경 전

```text
Product Details
Brewing Guide
Customer Reviews
Related Coffee Recommendations
```

### 변경 후

```text
Create concise sections for:

- Product Details
- Brewing Guide
- Customer Reviews
- Related Coffee Recommendations

Prioritize clean information hierarchy and avoid redundant content.
```

### 반영 이유

- 중복 정보 최소화
- 가독성 향상

---

## 9. 평점과 별점 일관성 확보

### 변경 전

```text
Customer Rating
```

### 변경 후

```text
Ensure customer ratings and star icons are visually consistent.
```

### 반영 이유

- 별점과 평점이 서로 다르게 생성되는 문제 방지

---

# v2 → v3 개선

v2 생성 결과를 분석한 결과 다음과 같은 한계가 발견되었다.

## 문제점

- 동일한 원두 패키지가 반복 생성됨
- 추천 상품의 개성이 부족함
- 실제 쇼핑몰 수준의 정보 구조가 부족함
- 로고와 패키지 구조가 페이지마다 조금씩 달라짐
- 메인 페이지 하단 콘텐츠가 부족함

---

## 개선 목표

### 1. 브랜드 일관성 강화

- 동일한 로고 사용
- 동일한 패키지 구조 유지
- 동일한 Typography 적용

---

### 2. 추천 상품 다양화

각 상품마다

- 원산지
- 패키지 색상
- 로스팅 단계

를 모두 다르게 지정하였다.

예시

| 상품 | 패키지 |
|-------|---------|
| Ethiopia Yirgacheffe | Cream |
| Colombia Supremo | Dark Green |
| Brazil Santos | Brown |
| Kenya AA | Black |

---

### 3. 중복 생성 방지

다음 네거티브 프롬프트를 추가하였다.

```text
Avoid duplicated product images

Avoid repeated package designs

Avoid inconsistent branding
```

---

### 4. 실제 쇼핑몰 구조 추가

메인 페이지에 다음 영역을 추가하였다.

- Best Sellers
- Customer Reviews
- Our Story
- Newsletter
- Footer

---

### 5. 브랜드 디자인 시스템 구축

모든 페이지에서

- 동일한 로고
- 동일한 패키지 구조
- 동일한 Typography
- 동일한 사진 스타일

을 유지하도록 프롬프트를 수정하였다.

---

### 결과

v3에서는

- 브랜드 일관성 향상
- 상품 중복 감소
- 콘텐츠 구성 확대
- 실제 쇼핑몰과 유사한 정보 구조
- 높은 완성도의 UI 디자인

을 확보할 수 있었다.
# 4. 최종(v3) 프롬프트 설계

v2 결과를 분석한 후 브랜드 일관성과 실제 쇼핑몰 구조를 강화하기 위해 프롬프트를 최종 수정하였다.

---

# 화면 1. 메인 페이지(Home)

## 목적

- 브랜드 첫인상 제공
- 대표 상품 소개
- 추천 상품 탐색 유도

## 주요 개선 사항

### 브랜드 일관성

- Home Barista 브랜드 고정
- 동일한 로고 사용
- 동일한 패키지 구조 유지

### Hero Section

- 대표 원두 상품 배치
- Espresso 이미지
- Wooden Cafe Background

### CTA

- Shop Now
- View All Products

### 콘텐츠 추가

- Recommended Coffee Beans
- Best Sellers
- Customer Reviews
- Our Story
- Newsletter
- Footer

### 디자인 요소

- Espresso Brown
- Cream Beige
- Warm White
- Soft Gold Accent

---

# 화면 2. 상품 목록(Product Listing)

## 목적

- 상품 탐색
- 상품 비교
- 필터 제공

## 주요 개선 사항

### Navigation

- White Navigation
- 동일한 로고
- 동일한 메뉴

### 상품 Grid

- 8개의 상품 카드

각 상품에는

- 상품명
- 원산지
- 가격
- 별점
- Add to Cart 버튼

을 포함하였다.

### 필터

- Single Origin
- Blend
- Decaf

### Sidebar

- Roast Level
- Origin
- Flavor
- Price

---

# 화면 3. 상품 상세(Product Detail)

## 목적

- 상품 정보 제공
- 구매 결정 지원

## 주요 개선 사항

### 메인 상품

Home Barista Ethiopia Yirgacheffe

메인 페이지와 동일한 패키지를 사용하도록 지정하였다.

### 상품 정보

- Product Name
- Price
- Origin
- Roast Level
- Rating
- Description

### Flavor Notes

- Chocolate
- Caramel
- Citrus
- Berry
- Floral
- Nutty

### Taste Bar

- Acidity
- Body

### CTA

- Fixed Add to Cart

### 하단 영역

- Product Details
- Brewing Guide
- Customer Reviews
- Related Products

---

# 공통 적용 사항

모든 화면에서 다음 항목을 동일하게 유지하였다.

- Home Barista Logo
- 동일 Typography
- 동일 Package Design
- 동일 Photography Style
- 동일 Navigation
- 동일 Color Palette

이를 통해 화면 간 브랜드 일관성을 확보하였다.

---

# 5. 이미지 후가공 프로세스

AI가 생성한 이미지를 그대로 사용하지 않고 후가공을 통해 완성도를 높였다.

| 대상 | 문제점 | 수정 방법 |
|------|---------|-----------|
| 공통 | 로고 형태가 페이지마다 다름 | 별도로 제작한 로고를 모든 화면에 동일하게 적용 |
| 공통 | 텍스트 깨짐 | Photoshop 및 Figma에서 텍스트 직접 수정 |
| 공통 | 메뉴 위치가 다름 | Content-Aware Fill을 사용하여 제거 후 동일한 위치로 재배치 |
| 상세 페이지 | 메인 페이지와 다른 상품 이미지 | Remove Background 기능으로 메인 상품을 추출하여 교체 |

---

## 후가공에 사용한 도구

- Leonardo AI
- Adobe Photoshop
- Figma

---

## 후가공 목적

- 브랜드 일관성 확보
- 텍스트 가독성 향상
- 실제 서비스 수준의 UI 구현
- 프로토타입 연결성을 고려한 화면 통일

---

# 결과

후가공을 통해

- 동일한 브랜드 로고
- 동일한 패키지 디자인
- 동일한 Navigation
- 동일한 Typography

를 적용하여 실제 쇼핑몰과 유사한 UI를 구현하였다.
# 6. Figma 연동 및 프로토타이핑 설계 로그

최종 디자인 시안을 Figma로 구현한 후 화면 간 이동이 가능한 프로토타입을 제작하였다.

---

# 6.1 프로젝트 정보

| 항목 | 내용 |
|------|------|
| 프로젝트 | Home Barista |
| 제작 도구 | Figma |
| 프로토타입 | Desktop Web |
| 화면 수 | 3개 |

---

## Figma Prototype

https://www.figma.com/proto/d2WzAMyN6b9P1UBFKRgKCY/Codyssey_B2-1?node-id=2-35&p=f&t=Z5sieIdpTmzVe4hR-1&scaling=contain&content-scaling=fixed&page-id=0%3A1

---

# 6.2 화면 구성

```text
Home
   │
   ├── Shop Now
   ▼
Product Detail
   ▲
   │
First Product
   │
Product Listing
```

총 3개의 화면으로 프로토타입을 구성하였다.

- Home
- Product Listing
- Product Detail

---

# 6.3 Hotspot 설계

| 순서 | 출발 화면 | 클릭 영역 | 이동 화면 |
|------|----------|-----------|-----------|
| 1 | Home | Shop Now | Product Detail |
| 2 | Home | Shop 메뉴 | Product Listing |
| 3 | Home | View All Products | Product Listing |
| 4 | Home | View All | Product Listing |
| 5 | Product Detail | 로고 | Home |
| 6 | Product Detail | Home 메뉴 | Home |
| 7 | Product Detail | Shop 메뉴 | Product Listing |
| 8 | Product Listing | 로고 | Home |
| 9 | Product Listing | Home 메뉴 | Home |
| 10 | Product Listing | 첫 번째 상품 | Product Detail |

---

# 6.4 사용자 흐름(User Flow)

```text
Home

 │

 ├───────────────┐

 ▼               ▼

Product Listing  Product Detail

 │               ▲

 └────상품 선택──┘
```

사용자는 메인 페이지에서

- 대표 상품 구매
- 상품 전체 보기

두 가지 흐름으로 이동할 수 있도록 설계하였다.

---

# 6.5 프로토타입 설계 목적

프로토타입은 실제 쇼핑몰의 사용자 경험을 최대한 반영하도록 설계하였다.

주요 목적은 다음과 같다.

- 화면 간 자연스러운 이동
- 실제 쇼핑몰과 유사한 UX 제공
- 발표 시 사용자 시나리오 시연
- 버튼별 역할 구분
- 사용자 동선 검증

---

# 7. 최종 결과

프로젝트에서는 Leonardo AI를 활용하여 Home Barista 브랜드의 UI 시안을 제작하였다.

프로젝트 진행 과정은 다음과 같다.

```text
서비스 기획

↓

프롬프트 설계

↓

Leonardo AI 이미지 생성

↓

Photoshop 후가공

↓

Figma UI 정리

↓

Prototype 제작

↓

최종 결과물
```

---

# 8. 프로젝트 회고

## 잘된 점

- 브랜드 아이덴티티를 일관되게 유지하였다.
- 실제 쇼핑몰 수준의 UI를 구현하였다.
- Figma 프로토타입을 통해 사용자 흐름을 검증하였다.
- 팀원 피드백을 프롬프트에 지속적으로 반영하였다.
- 후가공을 통해 AI 이미지의 한계를 보완하였다.

---

## 아쉬운 점

- AI 특성상 텍스트가 왜곡되는 문제가 발생하였다.
- 동일한 상품 이미지가 반복 생성되는 경우가 있었다.
- 로고 형태가 화면마다 조금씩 달라지는 문제가 발생하였다.

---

## 해결 방법

- Photoshop에서 텍스트를 직접 수정하였다.
- 로고를 별도로 제작하여 모든 화면에 동일하게 적용하였다.
- 대표 상품 이미지를 추출하여 상세 페이지에 재사용하였다.
- 프롬프트를 반복 수정하여 브랜드 일관성을 높였다.

---

# 9. 결론

본 프로젝트는 AI 기반 이미지 생성 도구와 Figma를 활용하여 프리미엄 커피 브랜드 **Home Barista**의 UI/UX 디자인 시안을 제작하였다.

Leonardo AI를 활용한 프롬프트 엔지니어링과 후가공 과정을 통해 브랜드 일관성을 유지하였으며, Figma 프로토타입을 활용하여 실제 서비스와 유사한 사용자 경험을 구현하였다.

또한 반복적인 프롬프트 개선과 팀원 피드백을 반영함으로써 초기 기획 의도를 효과적으로 시각화할 수 있었으며, AI를 활용한 UI/UX 디자인 프로세스의 실무 적용 가능성을 확인할 수 있었다.

---

# 사용 도구

| 구분 | 사용 도구 |
|------|----------|
| 이미지 생성 | Leonardo AI |
| 이미지 편집 | Adobe Photoshop |
| UI 편집 | Figma |
| 문서 작성 | Google Docs |
| 형상 관리 | GitHub |

---

# 프로젝트 구성

```text
Home Barista

├── README.md
├── docs
│   ├── 01_prompt_history.md
│   ├── 02_prompt_improvement.md
│   ├── 03_final_prompt_and_postprocessing.md
│   └── 04_figma_prototype.md
├── images
│   ├── home.png
│   ├── listing.png
│   └── detail.png
└── prompts
    ├── home_prompt.txt
    ├── listing_prompt.txt
    └── detail_prompt.txt
```
README.md
docs/
 ├── 01_prompt_history.md
 ├── 02_prompt_improvement.md
 ├── 03_final_prompt_and_postprocessing.md
 └── 04_figma_prototype.md
images/
prompts/
