# foundation-pure-html-page

[//]: # (## 서브모듈 등록)

[//]: # ()
[//]: # (- 현재 저장소에서, 서브모듈을 등록한다.)

[//]: # ()
[//]: # (```terminal)

[//]: # (// git submodule add <저장소URL> <저장될 폴더이름>)

[//]: # ($> git submodule add https://github.com/richfaber/foundation-pure-html component)

[//]: # (```)

- 동일한 스타일가이드를 가지는 n개 프로젝트 구성에서, `스타일 가이드 작업파일` 들이 논리적 연결이 되어, 프로젝트의 build 시 포함되어 배포되는 것이 목적이다.  
- 자원들은 `css, js, image` 를 의미한다.    
- 자원들이 프로젝트에 포함됨 으로써, 스타일가이드 자원을 프로젝트에 포함시키기 위한 별도 서버구성을 할 필요가 없다.
- 스타일가이드 저장소를 분리함 으로써, 독립적인 작업팀을 구성할 수 있다.    
- 서브모듈 관리를 통해서, 실수를 줄이고, 업데이트 내용을 손쉽게 프로젝트에 포함시킨다.

## 처음 클론 후

```terminal
$> git submodule update --init
$> git submodule foreach git checkout main
```

## 서브모듈 내용 업데이트 하기

```terminal
$> git submodule update --remote --merge
```

## 서브모듈 업데이트 포함 해서 클론 받기

```terminal
$> git clone --recurse-submodules https://github.com/richfaber/foundation-pure-html-page
```
