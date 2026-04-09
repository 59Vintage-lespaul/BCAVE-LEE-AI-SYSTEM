I have sufficient data now. Let me compose the final report.

# 리(LEE) 브랜드 DNA 추출 리포트

## 1. 읽은 자료 목록

| 상태 | 파일명 | 읽은 분량 | 주요 섹션 |
|---|---|---|---|
| [완독] `[Lee] Brand Introduction (KR) 250801.pdf` | 전 23p (2,3,5~22p) | B.CAVE 소개, History(1889~2019), Heritage 4대 아카이브(Union-Alls/Lee101/Lazy S/Buddy Lee), Products, Denim/Casual, Sales Channel(온·오프), ESG(indigood), Brand Collaboration 9건 |
| [완독] `✮[Lee] IP Guide_251028✮.pdf` | 전 6p | 로고 체계 (Main: 트위치 + Buddy Lee 심볼 / 1st Sub: 빈티지 / 2nd Sub: 하우스·신규(Vintage+Union) / Archive: Buddy Lee·Storm Rider·101) |
| [완독] `Lee_브랜드 아키텍쳐_종합_20260108(최종보고본).pptx` | 전 12슬라이드 (전문 텍스트 추출) | 로드맵, 2025 고객현황, 타겟전략·뮤즈(NCT 재민, 노윤서), 페르소나, 상품맵, 포지셔닝맵, 가격현황, 채널 현황(81.6→91.2억 vat-), 2021~2029 연혁 |
| [완독] `[Lee] 26SS 디자인,상품,소싱 기획안_250515(VSF).pdf` | 전 85p (전략 파트 집중 1~10, 21~22, 69~85) | 브랜드 피라미드, 포지셔닝맵, 시즌테마(SENSUOUS WORKWEAR), 컬러(Pantone), 그래픽 TO DO/NOT TO DO, 파이프라인 구분, 상품 기획(유니-시그니처/캐주얼/헤리티지, 우먼-Signature/K-Fashion Inspired/American Teenager, 악세서리), 25SS 히트 TOP10, CDQ(원가율 22.5→21.5%) |
| [완독] `LEE_26FW_ HQ 취합본.pdf` | 전 34p | 26FW 라벨/트림 라벨 체계 (BASIC ESSENTIAL / TREND / ACCENT ARCHIVE), 그래픽 마스터, UNI/WOMEN 아이템별 디자인 정리 |
| [완독] `[Lee] 25SS 디자인,상품,소싱 기획안.pptx` | 전 72슬라이드 (텍스트 추출) | ROAD MAP(피라미드 25 버전), Positioning Map, 24SS 리뷰, 컬러·원단, 그래픽 로드맵, 시즌테마(TIMELESS WORKWEAR), Key Styling(유니/우먼 데님·셔츠·스웨터), 상품 기획(생산 700억, 매출 407억), 카테고리 전략 |
| [부분] `[Lee] 25FW 디자인,상품,소싱 기획안_241115(VSF).pdf` | 1~10p | 25FW 로드맵 피라미드(동일 구조, 한글↔영어 버전), 포지셔닝 맵 (26SS와 동일) |
| [스킵] `[Lee] 24SS 상품,디자인,소싱 기획안_230601(Final).pdf` | - | 참고 우선순위 4단계, 시간 절약 위해 스킵 |
| [스킵] `LEE_24FW 디자인상품소싱기획안(VSF)_231117.pptx` | - | 지시사항에 따라 스킵 |

---

## 2. brand.config.json 초안

```json
{
  "brand": {
    "name": "Lee",
    "name_kr": "리",
    "slogan": "TBD (자료에서 미확인 — 고객 대면 슬로건 없음)",
    "tagline": "130년 전통의 미국 진즈웨어를 현재의 스타일로 재해석한다"
  },
  "identity": {
    "foundation": "USA · Workwear · Denim · History (브랜드의 기초이자 시작이었던 키워드)",
    "characters": ["교복화된", "미국적인", "트렌디한", "자유로운", "친근한", "근본있는", "가치있는", "브랜드 로고"],
    "principles": ["고객우선 (Customer First)", "자신감 (Pride)", "투명성 (ESG)", "주인의식 (Ownership)"],
    "north_star": "100년 전통의 미국 진즈웨어를 현재의 스타일로 재해석하여, 친근하고 세련된 근본있는 데님 캐쥬얼 브랜드가 된다",
    "design_concept": "American Denim Heritage reinterpreted for today (리의 헤리티지한 요소는 유지하면서 현대적인 느낌을 더하여 재해석)",
    "core_values": ["Heritage", "Denim", "Workwear", "Authenticity"]
  },
  "vision": {
    "statement": "데님을 필두로 라이프스타일 경험 확장을 통해 글로벌 헤리티지 패밀리 브랜드로 포지셔닝 공고화",
    "target_year": 2029,
    "milestone": "NO.1 글로벌 데님 헤리티지 패밀리 브랜드"
  },
  "positioning": {
    "axis": "DENIM ↔ CASUAL × CLASSIC ↔ TRENDY",
    "quadrant": "DENIM-TRENDY 사분면 (Lee 로고 위치)",
    "nearby_competitors": ["DIESEL", "Mod9", "Marithé François Girbaud"],
    "benchmark_brands": ["Polo Ralph Lauren", "Lacoste", "Calvin Klein"],
    "statement": "130년 넘는 브랜드 헤리티지를 데님 카테고리에서 공고화하고 프리미엄 정체성을 동시에 지향. 남녀·키즈·액세서리까지 포함한 패밀리 메가 브랜드로."
  },
  "strategy_2026": {
    "directions": [
      {
        "name": "데님 코어 강화",
        "from": "가성비 로고 캐주얼 이미지",
        "to": "데님을 코어로 둔 프리미엄 정체성 + 글로벌 헤리티지 브랜드"
      },
      {
        "name": "타겟 확장 (20대 유입)",
        "from": "30~40대 여성 중심 구매 구조 (여성 81%, 30~40대 69%)",
        "to": "20대 트렌드세터 메인 유입 + 30대 근본 브랜드 수요자 전환 + 40대 이상 기존 유지"
      },
      {
        "name": "대세감 IMC + 상품 기반 마케팅",
        "from": "로고 상품 집중 / 카테고리 킬러 / 셀럽 단발 마케팅",
        "to": "상품 기반 IMC(네이밍-육성), 레거시·트렌디 매체 통합 IMC, No.1 데님 스토리 집중, 매장·온라인 터치포인트 강화"
      },
      {
        "name": "시그니처 재정비",
        "from": "25SS 시그니처 고착화 (노후화, 기본 디자인 한정)",
        "to": "Basic FIt 재구축, 원단 고도화, 라벨/트림 체계화 (BASIC·TREND·ACCENT 3단 구조)"
      },
      {
        "name": "채널 질적 성장",
        "from": "샵인샵 82처 + 직영 2처 + 면세 4처 + 외부몰 중심",
        "to": "S·A급 유통 확장(더현대서울 등) 82→88처, FSS BEP 수준 상향, 자사몰 효율 강화, 명동 FSS 오픈(외국인 타겟)"
      }
    ]
  },
  "business_goals": [
    {
      "id": 1,
      "name": "데님 카테고리 리더십 확보",
      "tasks": ["시그니처 재정비 (Basic Fit 중심, 원단 고도화)", "헤리티지 아이템(카우보이 셔츠, 오버롤, 로고자켓) 확장", "데님 히트 아이템 부스팅 및 라인 세분화 (2027년 본격화)"],
      "kpis": ["TBD (자료에서 미확인)"]
    },
    {
      "id": 2,
      "name": "매출 912억 달성 (+11% vs 25년 816억)",
      "tasks": ["샵인샵 82→88처 확장", "직영점(FSS) BEP 달성, 명동 FSS 오픈", "자사몰 효율 강화"],
      "kpis": ["유통 매출 증가율 +12%", "신규 매장 +6개", "직영점 매출 +62%"]
    },
    {
      "id": 3,
      "name": "여성 고객 구조 재편",
      "tasks": ["우먼 라인 독립적 정규 시즌 컬렉션(Signature / K-Fashion Inspired / American Teenager)", "여성향 로고 베이직 핏 재정립", "가방 신학기 피칭 강화 (여성 고객 유입)"],
      "kpis": ["우먼 SKU 비중 +2%p", "우먼 매출 비중 +2%p", "우먼 생산 비중 20%"]
    },
    {
      "id": 4,
      "name": "제품 원가·품질 안정화 (CDQ)",
      "tasks": ["원가율 목표 21.5% 달성 (25SS 22.5% 대비 -1%p)", "납기 90% 이상 달성", "불량율 0.3% 이하 달성", "AIR 쿨링/기능성 원단 사용 확대"],
      "kpis": ["원가율 21.5%", "납기 달성률 90%+", "불량율 ≤0.3%"]
    },
    {
      "id": 5,
      "name": "20대 타겟 유입 확대",
      "tasks": ["아이돌 팬덤 기반 브랜드 인지 확대 (뮤즈: NCT 재민)", "20대 여성 중심 + 남성 타겟 확장 (뮤즈: 노윤서)", "숏폼/SNS 인플루언서 중심 IMC"],
      "kpis": ["TBD — 18~29세 Main Target KPI 미기재"]
    }
  ],
  "roadmap": {
    "2021": "Lee Korea 런칭 — 로고 상품 집중, 카테고리 킬러, 무신사 중심 온라인 확대",
    "2022": "브랜드 파이프라인 확립 — 전 카테고리 트렌디 이미지 확립",
    "2023": "여성 타겟팅 확장, 홍대 FSS 오픈, 여성 카테고리 확장·소싱력 강화",
    "2024": "오프라인 채널 확대, 자사몰 효율 강화, 효율적 유통망 확장(몰/아울렛)",
    "2025": "카테고리 확대 + 제품 IMC 강화 — 데님·하의류·시즌리스 상품 강화, 채널별 수익성 개선, 공간(SI) 경험",
    "2026": "대세 브랜드 마케팅 — 상품 기반 IMC(네이밍-육성), No.1 데님 스토리 집중, 레거시·트렌디 매체 통합 IMC, 매장·온라인 터치포인트 강화, 명동 FSS 오픈",
    "2027": "데님 본격 확장 / 데이터 고도화 — 히트 아이템 부스팅, 라인 세분화, 빅데이터·CRM 그로스 마케팅, 세분화 타겟팅",
    "2028": "라이프스타일 침투 — 브랜드 경험 확장(생활·문화), 글로벌 통합 캠페인, Top Tier 데님 캐주얼 브랜드 공고화",
    "2029": "글로벌 옴니채널 확장 — 마케팅 콘텐츠 APAC 프로덕션&매니징 진출, 데님 코어 글로벌 헤리티지 패밀리 브랜드 포지셔닝"
  }
}
```

---

## 3. personas.json 초안

```json
{
  "core_target": {
    "age_range_main": "18-29",
    "age_range_sub": "29-45",
    "definition": "트렌드를 이해하되, 각자의 방식으로 균형 잡힌 선택을 하는 동시대 소비자",
    "main_target_detail": "옷에 관심이 많고 브랜드의 가치와 감성을 이해하는 10대 후반에서 20대 후반",
    "sub_target_detail": "Lee가 가지고 있는 헤리티지를 느끼고 좋아하는 30대 초반에서 40대 초중반",
    "age_segments": [
      { "age": "19-23", "motivation": "팬덤 중심 유입 + 대세감", "strategy": "동조형 트렌드(컬러/핏) · 캐주얼 입문 · 아이돌 팬덤 기반 인지 확대" },
      { "age": "24-29", "motivation": "스타일 완성도 + 디테일/패턴/핏 (TRENDY)", "strategy": "20대 트렌드세터 타겟 확장 · 데님 팬츠 중심 스타일 제안" },
      { "age": "30-35", "motivation": "브랜드 헤리티지 + 30대 근본 브랜드 수요자", "strategy": "품질·리텐션 커뮤니케이션" },
      { "age": "36-45", "motivation": "품질 신뢰도 + 내구성/핏 (CLASSIC) + 충성도", "strategy": "스타일링 중심, 기존 고객 유지" }
    ],
    "muses_2026": [
      { "name": "NCT 재민", "role": "아이돌 팬덤 기반 브랜드 인지 확대 → 20대 초반 신규 유입" },
      { "name": "노윤서", "role": "20대 여성 중심 + 남성 타겟 확장, 데님 팬츠 중심 스타일 제안" }
    ]
  },
  "personas": [
    {
      "id": "male_lee_classic",
      "name": "검증 선호 남성",
      "description": "트렌드를 알지만 검증된 선택을 선호하는 남성",
      "age": 28,
      "gender": "male",
      "life_stage": "사회 초년생",
      "hobbies": ["맛집·술집 투어", "온라인 커뮤니티·숏폼 소비", "소규모 친목 러닝"],
      "preferred_brands": ["리바이스", "칼하트", "단톤", "랄프로렌"],
      "purchase_trigger": "지인·패션 커뮤니티 입소문 → 무신사에서 핏·리뷰 확인",
      "shopping_behavior": "오프라인 매장 착장 → 온·오프라인 병행 구매",
      "content_preference": "TBD (자료에서 미확인)"
    },
    {
      "id": "female_lee_balanced",
      "name": "균형 추구 여성",
      "description": "트렌드는 따르되 과하지 않은 균형을 찾는 여성",
      "age": 24,
      "gender": "female",
      "life_stage": "사회 초년생",
      "hobbies": ["카페 투어", "전시·팝업 방문", "라이프스타일 관련 콘텐츠 소비"],
      "preferred_brands": ["마리떼", "던스트", "빔즈보이", "유니클로U"],
      "purchase_trigger": "SNS(IG/YT) 인플루언서 영향 → 29CM에서 핏·리뷰 확인",
      "shopping_behavior": "오프라인 매장 착장 → 온라인 중심 구매",
      "content_preference": "TBD (자료에서 미확인)"
    }
  ],
  "data_insights": {
    "keyword_search_demographic_2025": {
      "female_pct": 81,
      "top_age_groups_pct": 69,
      "top_age_groups": "30-40대",
      "source": "네이버 데이터랩, 2025년 1~11월"
    },
    "offline_purchase_mix": {
      "uni_share_pct": 75,
      "women_share_pct": "TBD — 브랜드 아키텍처에 비중 표기 없음, 모수 적음(CRM 중요성 강조)"
    },
    "online_purchase_mix": {
      "uni_share_pct": 78,
      "women_share_pct": "TBD",
      "source": "세일즈 포스 + 자사몰 기준 (외부몰 향후 업데이트)"
    },
    "strategic_implication": "온·오프라인 모두 30~40대 여성이 구매 중심이나, 매출 구성은 UNI가 75~78%로 실제 고객 구조 대비 여성 상품군 비중이 낮은 불균형 구조. 20대 메인 유입·30대 소비 전환 강화·40대 이상 유지 단계적 설계."
  }
}
```

---

## 4. tone-manner.json 초안

```json
{
  "voice": {
    "personality": ["근본있는(Authentic)", "친근한(Friendly)", "세련된(Refined)", "헤리티지(Heritage-rich)"],
    "energy": "medium",
    "formality": "warm-confident",
    "humor_style": "TBD (자료에서 브랜드 유머 스타일 명시 없음)"
  },
  "language_rules": {
    "default_language": "ko",
    "gen_z_friendly": true,
    "avoid": [
      "옷 위에 그림을 그린 것처럼 보이는 그래픽 표현",
      "과도한 정밀 묘사",
      "과하게 카툰 같거나 귀여운 묘사",
      "칙칙하고 매력적이지 않은 컬러 구성",
      "구시대적이고 올드한 느낌",
      "가성비·저가 소구 (프리미엄 정체성 지향)"
    ],
    "prefer": [
      "깔끔하고 심플한 톤",
      "성별에 관계없이 공감할 수 있는 모티브",
      "세련되고 현대적인 컬러 조합",
      "가독성 높은 브랜드 이미지",
      "Lee 헤리티지를 유지하면서 현재의 트렌드를 감각적으로 접목"
    ],
    "hashtag_style": "TBD (자료에서 미확인)"
  },
  "channel_tone": {
    "instagram": { "tone": "TBD", "length": "TBD" },
    "tiktok": { "tone": "TBD", "length": "TBD" },
    "official_site": { "tone": "TBD", "length": "TBD" },
    "pdp_copy": { "tone": "TBD", "length": "TBD" }
  },
  "brand_vocabulary": {
    "must_use": ["Lee", "Heritage + Trend", "130년 전통", "데님", "워크웨어", "Buddy Lee", "Lee 101", "Lazy S", "Union-Alls", "indigood"],
    "never_use": ["저렴한", "가성비", "짝퉁", "평범한"]
  },
  "graphic_guideline": {
    "to_do": [
      "어패럴·용품에 적용 시 난해하지 않고 깔끔, 심플한 그래픽 디자인 추구",
      "전반적 컬러감 구성이 매력적이며 세련되고 현대적인 컬러 조합 구현",
      "메인 BI를 활용해 가독성 높은 브랜드 이미지 전개",
      "성별 관계없이 공감할 수 있는 모티브를 활용한 트렌디한 아트웍 제작"
    ],
    "not_to_do": [
      "옷 위에 그림을 그린 것처럼 보이는 그래픽은 최대한 배제, 과도한 정밀 묘사 지양",
      "과하게 카툰 같거나 귀여운 그래픽 지양",
      "칙칙하고 매력적이지 않은 컬러 구성 피할 것",
      "구시대적이고 올드한 느낌의 아트웍 배제"
    ]
  }
}
```

---

## 5. visual-identity.json 초안

```json
{
  "design_keywords": ["Denim Heritage", "Workwear", "American Authentic", "Clean & Simple", "Modern Refined"],
  "mood": "Lee가 가지고 있는 헤리티지한 요소는 유지를 하면서 현대적인 느낌을 더하여 재해석",
  "logo_system": {
    "main": {
      "logo_type": "Lee 트위치 로고 (Twitch logo)",
      "symbol_type": ["Buddy Lee 전신 캐릭터", "Buddy Lee 얼굴 심볼"],
      "rules": [
        "1번 표시 형태가 기본",
        "자수의 경우 10cm 이하는 R 빼고 작업",
        "프린트의 경우 모두 R 있는 로고 사용",
        "3.4cm 로고 프린트 작업 시 R이 큰 전용 로고 사용",
        "R / MR / MS / USA / 누끼 / 박스 등 변형은 디자인 재량이나, 변형 진행 시 컨펌 후 진행"
      ],
      "variants_count": 10
    },
    "first_sub": {
      "logo_type": "Vintage 로고 (Lee 빈티지 세리프형)",
      "note": "LEE에서 사용하던 기본 빈티지 로고 형태. 1번을 주로 사용하나 이외 사용은 디자이너 재량. 변형 진행 시 컨펌 후 진행"
    },
    "second_sub_house": {
      "logo_type": "House 로고 (삼각 지붕 + Lee)",
      "rules": [
        "1,2 표시 형태가 기본",
        "박스 분할 / 워딩 추가 및 변형 / 디자인 변형 재량",
        "**워크웨어 관련 그래픽** 제외 사용 지양 (ex. 카우보이·버디리 그래픽 등 워크웨어 관련 아닌 그래픽에 같이 사용 지양)",
        "베이직 아이템 등은 사용 가능"
      ],
      "variants": ["KANSAS CITY U.S.A", "WORK CLOTHES", "TRADE MARK REG. Established. 1889", "PREMIUM QUALITY"]
    },
    "second_sub_new": {
      "logo_type": "신규 로고 (LEE KOREA 개발)",
      "variants": [
        { "name": "VINTAGE LOGO", "description": "세리프 블록