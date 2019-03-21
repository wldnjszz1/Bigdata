[[ 아나콘다 다운로드 ]]
window + R
입력 : \\M1503INS 후 엔터
빅콘테스트Data 진입
ana.exe 다운로드 
-----------

1. 기존 python.org로 설치한 python 제거
   굳이 않지워도 되나, 중복성이 있어서 한개만 설치로
   진행
2. 아나콘다 설치 (path 체크 주의)
3. 주피터 구동
   주피터는 ipython(분석용 툴) 기반으로 flask로
   만든 웹기반 에디터 => 분석 IDE로 사용
   1) 콘솔에서 jupyter notebook 구동
   2) 아나콘다 메뉴에서 jupyter notebook 클릭
   3) 해당 프로젝트에서 bat(sh)을 만들어 구동
      ---------
      echo '주피터 가동'
      jupyter notebook
      pause
      ---------
4. 셋업
   anaconda navigator 구동
   environments 클릭
   create > 가상환경명 지정 > 파이썬버전 선택
   home > 가상환경 선택 확인 > 주피터 노트북 install
   > 주피터 노트북 런치
   --------------------------------------------------

5. 데이터 분석 과정
  > 기획, 요구사항 분석 
  > 데이터 수집-> 전처리 -> 적제(DB, csv,...)
    => 70%
    => 0단계 누가 제공해주면 OK( 공공데이터 )
       주소, xml, json, csv 등등 파싱하는 방법
    => 1단계 API
    => 2단계 scraping : beautifulsoup4
    => 3단계 crawling
    => 4단계 패킷분석
  > 데이터 분석 (시각적(데이터속성 파악), 통계적)
    => 예측을 하나 통계적인 수단
  > 예측 : 머신러닝, 딥러닝
    데이터 -> 학습 -> 모델구축 -> 예측 -> 정확도!!  
  > 빅데이터 분석
    시스템구축(하둡,클러스터) 
    -> 아파치 스파크(스칼라 or 파이스파크 or 스파크 R) 
    -> 실시간 수집 -> 분석 or 머신러닝 -> 분석결과,예측
  > (최종단계) 시스템 통합
   -> 기존 시스템에 기능 추가등 통합 or
   -> 신규 서비스 생성 or
   -> 보고서/ppt
    
6. 세팅(추후라도 추가하면 반드시 requirements.txt를 갱신)
 아나콘다 네비게이터 > environments > DataAnalysis > 화살표 > open Terminal
 각자 프로젝트 위치로 이동
 
 이동 후 프럼프트
 (DataAnalysis) C:\Users\LG\Desktop\py_projects\data_crawling>
 
 한번에 프로젝트에 사용하는 패키지를 일괄 설치한다
 (DataAnalysis) 길어서 줄여씀 > pip install -r requirements.txt
 
 확인
 (DataAnalysis) > pip list
 
 만약 누락이 있으면 
 pip install 모듈명
 
 7. API 방식 진행시
 > Postman 프로그램을 이용해 요청만 전문으로 테스트
  => 잘 진행되는지 체크