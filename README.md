# foundation-pure-html-page

[//]: # (## 서브모듈 등록)

[//]: # ()
[//]: # (- 현재 저장소에서, 서브모듈을 등록한다.)

[//]: # ()
[//]: # (```terminal)

[//]: # (// git submodule add <저장소URL> <저장될 폴더이름>)

[//]: # ($> git submodule add https://github.com/richfaber/foundation-pure-html component)

[//]: # (```)

n개 프로젝트 구성에서, 스타일가이드의 작업분이 논리적 연결이 되어야 한다.  
이렇게 프로젝트에 종속된 스타일가이드는, 프로젝트 build 에 포함되어, 배포된다.

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
