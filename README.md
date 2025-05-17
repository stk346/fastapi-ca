* poetry로 프로젝트 만들기
    * 가상환경 설정
        * poetry init
    * 가상환경 구동
        * poetry shell
    * .toml 파일에 설정된 패키지 설치
        * poetry install

* pyenv로 가상환경 활성화 및 파이썬 설치
    * brew install pyenv
    * pyenv install 3.10.13
    * 프로젝트 루트에서 python 버전 지정
        * pyenv local 3.10.13
        * poetry env use $(pyenv which python)

* fastAPI 설치
    * poetry add fastapi

* 유비콘
    * 유비콘 설치
        * poetry add "uvicorn[standard]"
    * 유비콘으로 서버 구동 (poetry 가상환경 실행한 상태에서 명령어 실행 )
        * uvicorn main:app --reload --port 8000