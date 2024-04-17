> **해표면 물질 궤적 모의 및 예측[팀]**

*2023.09.06 - 2023.11.24*

제3 해양과학 빅데이터 공모전에서 진행한 해표면 물질 이동경로 예측 프로젝트 관련 코드입니다.

**‘’기상데이터를 이용해 다양한 통계론적 방법 적용”**

### [목적]

- 2005년 동해에 위치했던 31개의 표층 뜰개 궤적 모의 및 새로운 7개 뜰개의 궤적 예측

### [인원]

- 3명 - 수학과 학부생 2명, 감염병 확산 수리모델링 연구원 1명

### [역할]

- DTW, Ward 연결방법 이용해 31개의 뜰개 궤적을 3종류로 군집화
- 오픈API를 활용해 31개 뜰개의 궤적에 해당하는 기상데이터 구축
- 격자 형식의 기상데이터에 Bilinear Interpolation를 적용해 특정한 경도, 위도의 기상데이터 생성
- Pandas의 DataFrame 대신 Xarray 모듈을 사용해 다차원 기상데이터 접근 시간복잡도를 기존 대비 20% 감소시킴
- XGBoost 모델을 사용해 단일 Step 예측의 반복으로 100일간의 뜰개 궤적 예측

### [사용 기술]

- 언어: Python
- 라이브러리: Tensorflow, Scikit-learn, Xgboost, Cartopy, Seaborn, Scipy
- API: Copernicus Marine  Service, CDS API
- 개발 환경: Intel i7 RAM 8G, NVDIA GeForce GTX 1050 VRAM 4G

### [성과]

- 한국해양수산과학기술진흥원 주관 제 3회 해양과학 빅데이터 경진대회 종합 리더보드 7등 달성

관련 링크
https://haebomdata.notion.site/ec77b916b9c84d309f1a363b1d18a16d

