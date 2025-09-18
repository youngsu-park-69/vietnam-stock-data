# 🇻🇳 베트남 상장기업 데이터베이스

베트남 증권시장 전체 1,638개 상장기업의 종합 데이터베이스

## 📊 데이터 개요

- **HOSE**: 393개 기업 (호치민 증권거래소)
- **HNX**: 341개 기업 (하노이 증권거래소)  
- **UPCOM**: 904개 기업 (장외시장)
- **총계**: 1,638개 기업

## 📁 파일 구조

vietnam-stock-data/
├── README.md
├── data/
│ ├── vietnam_companies.csv # 전체 1,638개 기업
│ ├── vietnam_companies_hose.csv # HOSE 393개
│ ├── vietnam_companies_hnx.csv # HNX 341개
│ └── vietnam_companies_upcom.csv # UPCOM 904개
└── scripts/
└── db_import_guide.md

text

## 🔗 직접 사용 URL

전체 데이터 다운로드
curl -O https://raw.githubusercontent.com/youngsu-park-69/vietnam-stock-data/main/data/vietnam_companies.csv

text

## 📈 n8n에서 사용법

{
"url": "https://raw.githubusercontent.com/youngsu-park-69/vietnam-stock-data/main/data/vietnam_companies.csv",
"method": "GET"
}

text

## 📋 데이터 필드

- `symbol`: 주식 심볼
- `name`: 영문 회사명  
- `name_vn`: 베트남어 회사명
- `exchange`: 거래소 (HOSE/HNX/UPCOM)
- `sector`: 섹터
- `industry`: 세부 업종
- `market_cap_class`: 시가총액 등급 (LARGE/MID/SMALL)
- `market_cap_vnd`: 시가총액 (VND)
- `market_cap_usd`: 시가총액 (USD)
- `is_vn30`: VN30 지수 포함 여부
- `is_dividend_stock`: 배당주 여부
- 기타 27개 필드...

## 🗂️ 업데이트 이력

- 2025-09-18: 초기 데이터베이스 구축 (1,638개 기업)
