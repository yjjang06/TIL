# git, GitHub 기초
이전에 회사에서 git을 사용해본 경험이 있어서 간단하게 수업 내용 정리해보았습니다.
평소에는 GUI 환경에서 주로 작업했지만, CLI 환경에서 실습해보니 새로운 경험이었습니다.

## Conventional Commits
- [Conventional Commits](https://www.conventionalcommits.org/ko/v1.0.0/)
- 명확한 커밋 히스토리를 생성하기 위한 간단한 규칙
- prefix 종류
	- feat : 기능 개발 관련
	- fix : 오류 개선 혹은 버그 패치
	- docs : 문서화 작업
	- conf : 환경설정 관련

## .gitignore
- Git에서 **버전 관리하지 않을 파일이나 폴더, 파일 패턴**을 지정하는 설정 파일
- [Toptal](https://www.toptal.com/developers/gitignore/)에서 원하는 설정에 맞는 .gitignore 파일 생성이 가능

## pre-commit
- commit 수행  전  체크해야  할  것들을  자동수행하도록  도와주는  도구
```shell
# MacOS 환경에서 실습

$ pip --version # pip 존재 확인
$ pip install pre-commit # 설치
$ pre-commit -V # 명령어 존재 확인
$ pre-commit sample-config > .pre-commit-config.yaml # 샘플 설정 만들기 $ pre-commit run # 실행 확인
```
- 설치 후 바로 실행이 되지 않아 환경변수 설정 추가
```shell
$ sudo vim ~/.zshrc
# export PATH="$HOME/.local/bin:$PATH" 추가 후
$ source ~/.zshrc # 실행
```
