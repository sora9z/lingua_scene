## 가상환경 도구

- 가상환경 도구 설치
  pip install pipenv

- 가상환경 생성
  pipenv --python 3.12.\*

- 가상환경 삭제
  pipenv --rm

- 가상환경 실행
  pipenv shell

## 프로젝트 생성

- 프레임워크 설치 pip install django
- 아래 명렁어는 현재 폴더를 프로젝트 자체로 사용하겠다는 의미.

```
  django-admin startproject config .
```

## 패키지 설치

- rest framework 설치

  ```
  pipenv install djangorestframework
  ```

- isort, black, flake8 설치

  - 코드 품질을 향상 시키고 협업시의 코드 작성 스타일 등에 따른 충돌 문제등을 예방하기 위함

  ```
  pipenv install isort black flake8
  ```

  - isort는 파이썬 코드의 import 구문을 자동으로 정렬해주는 도구
  - black은 파이썬 포멧터로 일관된 코드 스타일로 변환시켜줌 PEP8기준
  - flake8은 코드스타일 문제, 문법오류, 잠재적인 버그 확인해주는 도구
  - isort와 black을 pyproject.toml로 설정하고 flake8의 설정은 .flake8으로 설정하

- pre-commit 설치
  - commit 전에 자동으로 수행될 수 있게 해주는 패키지

```
pipenv install pre-commit
```

- pre-commit 설정파일 생성 및 설정 (.pre-commit-config.yam)
- pre-commit hook 생성

```
pre-commit install
```

## 6. github 연결하기

- my_settings.py : secrete key 분리
