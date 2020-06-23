# 부산대학교 한국어 문장 분석 시스템 BCD-KL-Parser
- 원활한 진행을 아래 개발환경을 참고하여 주시기 바랍니다.

## 본 연구진의 한국어 구문분석 전략
- 생성 문법: 의존문법(dependency grammar)
- 형태소 분석 결과의 활용: 모든 형태소분석 후보를 활용
- 구문분석 단위: 형태소
- 구문분석 방법: 차트 파싱(chart parsing)
- 구문분석 출력 결과: 구문분석 트리 후보를 순위화하여 출력

### 특징(1) - 규칙 기반 문장분석
- 자연스러운 지식 표현 / 처리 과정과 지식의 분리
- 빠른 처리 속도
- 학습 말뭉치가 불필요함
- 응용영역과 무관한 시스템 구현 가능
- 불완전하고 불확실한 지식(예외 현상 처리 포함)을 다룰 수 있음
- 설명 가능 인공지능(Explainable Artificial Intelligence; XAI)

### 특징(2) - 형태소 단위의 문장분석
- 어절 단위와 비교하여 더 적은 데이터로 효과적인 모형의 개발이 가능
- 모든 형태소 분석 결과를 활용하여 오류 전파 문제에 강건함

### 특징(3) - 차트 파싱
- 1-way 알고리즘
- 모든 형태소 분석 결과를 이용하는 문장분석에 적합함

## 개발환경
- IDE: Microsoft Visual Studio Community 2017
  - 워크로드에서 'C++를 사용한 데스크톱 개발' 포함
  - 개별 구성요소에서 '컴파일러, 빌드 도구 및 런타임 > Windows 유니버설 CRT SDK' 포함
- 언어: C++ and C#

## 프로젝트 구성
- 형태소 분석기 – 동적 라이브러리(PnuNlpCore.dll)
- 품사 태거 – 동적 라이브러리(KLTagger.dll)
- 구문 분석기 – 소스코드

## 프로젝트 빌드/실행 방법
1. 본 저장소에서 '[Develop]KLParser3.7.3(2020.06.23).zip'를 내려받은 후 압축해제
  - 다운로드 속도 문제로 본 저장소에서 소스코드만 포함
2. 아래 경로에서 '[Develop]KLParser3.7.3(2020.06.23)_exe.zip'를 내려받은 후 1에 덮어쓰기
  - http://ailab.iptime.org/sharing/jum0Omyyc
  - 프로그램 실행만 원하시면 2번만 진행
3. 관리자 권한으로 VS 2017 실행 후 1의 솔루션 파일 열기
  - 내부 결과를 레지스트리에 저장하기 때문에 관리자 권한 필요
4. 'Parser4CSharp'를 시작 프로젝트로 설정 후 빌드/실행

## 문의
- 이메일 : kst8798@gmail.com(연구원) / aidocu@pusan.ac.kr(연구실)

