# 김유겸
#포트폴리오

#C언어 관련 작업

#연구실 급


#1. 1차원 윷놀이 승리전략 시뮬레이션 초기에 확률계산 및 전략 논리구조에 관한 소스 개발 도움 및 수정.
#

   데이터 수집 및 분류에 관한 프로그램 개발 도움. (학부연계 연구였던 직접적인 연구에는 참여 하지 않음.)

 - Analysis of the One-dimensional Yut-Nori Game: Winning Strategy and Avalanche-size Distribution 논문 

 1차원 윷놀이 게임의 모든 경우의 수에 대한 확률을 계산하는 프로그램을 기반으로 사각형 윷놀이, 기본 윷놀이
 게임에 대한 확률을 계산하는 프로그램 개발. 5개의 교차점과 상대의 말을 잡는 부분의 확률계산 오류를 잡기위해
 각 확률의 직접적인 계산방법과 각 말을 움직이는 확률을 독립적으로 계산해 오류를 검증하게 했습니다.



#2. 유전연구실의 유전알고리즘을 석사생 연구용으로 수정 및 프로그램 구조 해석 & 설명, 보완
#

 5000줄 가량의 기존 파이썬으로 쓰여진 유전알고리즘의 요소를 해석하여 논리 구조, 각 함수와 변수의 의미를 2명의 연구생

에게 설명하고 수행시간과  연구목표에 따라 C언어로 포팅하는 과정에서의 수정점과 이유에 대해 가르쳤습니다. 

 더하여 일주일 정도의 시간동안 각자가 수정한 코드의 오류에 대하여 피드백을 진행했습니다. 



#3. 인지과학 연구실 동공운동 데이터 분석 프로그램 효율 개선 및 패턴에 따른 분류 코드 추가.
#

 Visual Basic 코드로 이루어진 기존 데이터 분석 프로그램 소스에 처리속도 증가와 데이터 분류를 목적으로 소스코드를 작성 

했습니다. 

 시계열 좌표로 이루어진 데이터를 중심점에 대한 원주좌표로 변환해 운동 데이터의 크기 및 연산 속도를 향상 시켰으며 운동 

양상에 따라 유사 패턴 별로 추출하여, 글리치 정리 정확도를 향상시켰습니다.

 제가 작성한 C언어 코드를 모듈화 하고 DLL 파일과 적용에 관해서는 기존 프로그램을 관리하던 분이 작업했습니다.



#4. 연음반복통계에 따른 푸리에 급수를 이용한 음원 분석, 장르구분 프로그램 작성 
#

 mp3파일의 압축된 Wave 데이터를 Rosetta Code에 등재되어 있는 Fast Fourier transform(FFT) 소스를 이용하여 시계열 주파

수 데이터로 변환하고 시계열 데이터의 시간간격을 이용해 음의 높낮이를 추출했습니다.

 추출된 음에 대응하는 음계에 따라 연음 관계에 있는 데이터들의 빈도수와 시간상의 배치에 대한 통계 데이터를 아웃풋하여 

각 장르별 유사성을 비교하는 기능을 수행하게 했습니다. 

 초기에 음의 빈도수에 대한 통계에서는 장르 내 유사성이 발견되지않아 연음에 대한 통계를 관찰 하는 것으로 방향을 수정 

하였으며 연은 통계에서는 장르내 유사성 및 장르간 패턴 차이를 발견할 수 있었습니다.



#5. 사회 모델 네트워크 초기값 생성(10만 개의 표본 노드와 사이의 관계 링크 생성) 프로그램 작성.
- 사회 모델 네트워크를 이용한 전염확산 기저 및 병의 성질에 따른 전파 양상 분석 프로그램 작성.
- 이미 연구 결과가 있는 주제에 대한 시뮬레이션 모델 개발 작업.
#

 척도없는 네트워크 상에서 전염확산의 양상에 대한 연구결과를 기반으로 시뮬레이션을 구현했습니다. 

각 노드를 개인으로 상정하고 좌표, 면역력, 사회성 인자를 가진 구조체로 설계하였으며 사회성 인자를 기반으로 링크를 연결

해 Scale-free 결합수 분포를 가지는 네트워크를 생성하는 프로그램을 제작했습니다. 

더불어 생성된 네트워크 상에서 랜덤하게 질병을 발병시켜 첫 발병 노드의 링크수와 클러스터 인접도에 따른 확산 및 유지, 

병의 사멸에 대한 통계 지표를 얻는 프로그램을 따로 작성했습니다.

#학술동아리 급

#1. 3체 운동 시뮬레이션 모델 오차 수정, 튜닝을 통한 속도개선.
#

 3체 운동의 안정성을 확인하기 위한 시뮬레이션에서 안정화 되어야 하는 초기값에서도 발산하는 결과를 내는 프로그램을 

Runge-Kutta 4th Mthd를 사용해 오차를 줄이고 중간 연산과정에서의 유사성을 이용해 계산과정을 한단계 줄였습니다.
 
#2. 팀 프로젝트 - 5요소 먹이사슬 시뮬레이션 모델 개발 및 로직 수정, 오류 검수.
#

 풀, 토끼, 사슴, 여우, 늑대로 이루어진 먹이사슬 시뮬레이션을 통해 기본적인 요소(번식, 이동, 섭취) 만을 가진 개체를 시

뮬레이션 했을 때 개체수가 복잡한 네트워크의 특징인 멱함수 형태가 나타나는 지 확인해 보기 위한 프로젝트였습니다.

 수직적 먹이사슬인 경우에는 예측 가능한 범위내에서의 개체수 변동만을 관측할 수 있었기 때문에 수직적 먹이사슬에서 벗어

난 수평적 경쟁관계(토끼, 사슴)를 추가한 모델로 수정 했으며 4가지 상수를 가지는 멱함수 분포를 확인할 수 있었습니다.

 
