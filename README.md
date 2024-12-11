# 특허 데이터 기반 데이터처리 기술 트렌드 분석

이 프로젝트는 특허 데이터를 활용해 디지털 데이터 처리 기술의 주요 트렌드와 키워드를 분석한 내용을 담음. LDA 토픽 모델링과 클러스터링 분석을 통해 기술 간의 연관성과 변화 추세를 확인함.

## Project Period
2024.04.10 ~ 2024.06.30

## Team
- 데이터사이언스학과 2021111716 김송연
- 데이터사이언스학과 2021111741 조인아
- 데이터사이언스학과 2022111744 안교영

## 프로젝트 구조
- **`notebooks/`**: 분석 과정을 단계별로 기록한 Jupyter Notebook
  - `1_api_data_collection.ipynb`: 특허 데이터를 API를 통해 수집
  - `2_eda.ipynb`: 결측치 및 데이터 탐색 진행
  - `3_preprocessing_modeling.ipynb`: 텍스트 전처리, 토픽 모델링, 시각화를 수행
- **`data/`**:
  - `raw/`: 수집된 원본 데이터 저장
  - `processed/`: 전처리된 데이터 저장
- **`results/`**:
  - `visualizations/`: 분석 결과의 시각화 자료
  - `reports/`: 최종 보고서
- **`README.md`**: 프로젝트 설명
- **`requirements.txt`**: 프로젝트 실행에 필요한 라이브러리
## 목표
1. 특허 데이터를 활용해 디지털 데이터 처리 기술의 주요 토픽과 트렌드를 분석함
2. 도출된 결과를 통해 기술 간 연관성과 변화 추세를 시각화함
3. 클러스터링 및 네트워크 분석으로 유사 기술 그룹을 도출함

## 분석 파이프라인
1. **데이터 수집**:
   - KIPRIS Plus API를 활용해 특허 데이터를 수집함
   - 수집 데이터: 출원일, 초록, 발명의 명칭, IPC 번호 등
2. **데이터 전처리**:
   - 텍스트 정제 및 토큰화 진행 (Okt 사용)
   - 불용어 제거 및 텍스트 데이터 클리닝
3. **토픽 모델링**:
   - LDA 모델을 통해 주요 토픽을 추출하고 키워드별 인사이트를 도출함
   - 토픽별 연도 분포와 특허 개수를 분석함
4. **클러스터링 및 네트워크 분석**:
   - K-means 클러스터링으로 유사 토픽 그룹화
   - 네트워크 시각화로 토픽 간 연관성을 확인함
5. **결과 도출**:
   - 각 토픽별 핵심 키워드와 특허 트렌드를 기반으로 주요 인사이트를 제시함

## 주요 결과
1. **토픽별 키워드**:
   - 사용자 인터페이스, 데이터 보안, 터치스크린 및 센서, 이미지 및 영상 처리 등 다양한 기술이 도출됨
2. **트렌드 분석**:
   - 데이터 보안과 개인정보 보호 관련 주제(Topic7)가 점진적으로 증가하는 추세를 보임
   - 터치스크린 기술(Topic5)은 상대적으로 감소하는 경향을 보임
3. **클러스터링**:
   - 토픽 간 유사도를 기반으로 하드웨어, 소프트웨어, 기반 기술 그룹으로 구분됨


