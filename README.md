# 아나콘다 설치하기 (Mac)
- 아나콘다: 머신러닝이나 데이터 분석 등에 사용하는 여러가지 패키지가 기본적으로 포함되어 있는 파이썬 배포판, 파이썬 가상 환경을 구축하는데도 유용하게 사용 가능
- https://www.anaconda.com/download#macos에서 mac용 설치 프로그램 다운로드
- Terminal 열기
- 콘다 버전 확인 및 업데이트
  - conda --version
  - conda update conda
- 프로파일 업데이트
  - source ~/.bash_profile
- 새로운 가상환경 생성하기
  - conda create --name "가상환경명" python="파이썬버전"
- 가상환경 삭제하기
  - conda remove --name "가상환경명"
- 가상환경 목록 확인하기
  - conda info --envs
- 생성한 가상환경 활성화하기
  - conda activate "생성한 가상환경명"


# jupyte notebook과 vscode 연결하기
- 플러그인 설치
  - vscode에서 Jupyter 플러그인 설치 (Extension Pack임, 4개)
  - vscode에서 Python 플러그인 설치 (Pylance 함께 설치됨)
- 새파일 만들기
  - Shift + Command + P (사용할 수 있는 모든 commands 보여줌)
  - Create: New Jupyter Notebook 선택
  - Command + S (저장)
- 파이썬 인터프리터 선택하기
  - Python: Select Interpreter 선택
  - 원하는 인터프리터 선택
- 참고: Jupyter Notebook 파이썬 인터프리터 default 설정하기
  - Command + , or Code -> 기본 설정 -> 설정 찾아 들어가기
  - 검색창에 python이라고 침
  - Python: Default Interpreter Path에서 Path 설정해주기 (ex> /Users/buzzni/anaconda3/bin)

   
# Mac에서 jupyter notebook 설치하기
- Terminal 열기
- pip3 install --upgrade pip
- pip3 install jupyter
- jupyter notebook

# 가상환경에서 jupyter notebook 실행할 경우
- jupyter notebook에 가상환경 연결해야 함
- python -m ipykernel install --user --name {가상환경 이름} --display-name "{디스플레이 이름}"
  - ex> python3 -m ipykernel install --user --name test --display-name test
  
# conda 가상환경에 pytorch 설치
- 가상환경 생성
- https://pytorch.org/get-started/locally/ 에서 설정 후, Run this Command를 복사해서 실행
  - ex> conda install pytorch::pytorch torchvision torchaudio -c pytorch




