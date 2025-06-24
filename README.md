# 🛒 당근마켓 크롤링 및 지역 기반 커뮤니티 분석

본 프로젝트는 **당근마켓(Daangn)**에서 특정 키워드를 기반으로 **중고 상품 게시글 데이터를 수집**하고,  
이를 바탕으로 **지역별 커뮤니티 활동 분석 및 토픽 모델링**을 수행한 **크롤링 + 데이터 분석 통합 프로젝트**입니다.

---

## 📌 프로젝트 목적

- **1단계: 크롤링**
  - 사용자가 입력한 키워드에 대해 당근마켓 게시글 데이터를 수집 (제목, 내용, 이미지, 지역, 링크 포함)
  - 동적 페이지 로딩 및 더보기 버튼 자동 클릭 구현

- **2단계: 지역 분석**
  - 수집된 게시글에서 `region` 정보를 추출하여 **지역별 글 개수 시각화**
  - `GeoPandas`를 활용해 지도에 시각적으로 매핑

- **3단계: 토픽 모델링**
  - `Okt` 형태소 분석기를 이용해 게시글 본문 텍스트 전처리
  - `LDA(Latent Dirichlet Allocation)` 모델을 활용하여 **러닝크루 게시글의 주요 관심 주제 추출**

---

## 🧰 사용된 기술 스택

| 분류            | 라이브러리/툴                         |
|-----------------|--------------------------------------|
| 크롤링          | Selenium, BeautifulSoup              |
| 데이터 처리     | pandas, re                           |
| 지도 시각화     | geopandas, matplotlib                |
| 형태소 분석     | konlpy (Okt)                         |
| 토픽 모델링     | gensim (LDA), tqdm                   |
| 기타            | ipywidgets, warnings, pickle         |

---



## 📄 License
This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

