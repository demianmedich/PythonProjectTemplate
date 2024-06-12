# PythonProjectTemplate

초기 파이썬 프로젝트의 구조를 빠르게 설정하기 위해 만든 파이썬 템플릿 저장소입니다. 

## How to use
### 1. venv setup
PyCharm에서 virtualenv 셋업을 별도로 진행할 경우 스킵
```bash
$ pip install virtualenv
$ python -m virtualenv <venv dir>
$ source <venv dir>/bin/activate
```

### 2. 파일 수정
- `src/` 아래에 파이썬 패키지 추가하기  
```bash
$ mkdir src/<mypkg>
```
- pyproject.toml 수정하기
```toml
[project]
name = "Fix me"  # src/ 아래에 생성한 패키지 명과 동일하게 수정
version = "0.0.1"
```

### 3. 패키지 설치하기
```bash
$ pip install --upgrade pip
$ pip install setuptools  # build backend로 setuptools 사용
$ pip install -e .[dev]  # editable 모드로 설치
```
zsh 사용자의 경우 `.[dev]`를 `".[dev]"`로 수정


