# foundation-pure-html-page

foundation-pure-html 의 컴포넌트 스타일을 서비스에 포함시키기 위해서 서브모듈 등록 한다.

## 요구사항

- 물리적 파일이 실제로 포함되서 번들이 되고, 업데이트 내용도 손쉽게 관리하길 원함

## 서브모듈 등록

- 현재 저장소에서, 서브모듈을 등록한다.

```terminal
// git submodule add <저장소URL> <저장될 폴더이름>
$> git submodule add https://github.com/richfaber/foundation-pure-html component
```

## 처음 클론 후

```terminal
$> git submodule update --init
$> git submodule foreach git checkout main
```

## 서브모듈 업데이트 포함해서 클론 받기

```terminal
$> git clone --recurse-submodules https://github.com/richfaber/foundation-pure-html-page
```

## 서브모듈 내용 업데이트 하기

```terminal
$> git submodule update --remote --merge
```
