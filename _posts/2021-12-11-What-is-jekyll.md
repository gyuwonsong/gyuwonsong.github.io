---
layout: post
title: jekyll
date: 2021-12-11 02:34 +0800
tags: 
- jekyll
- what_is_jekyll?
- github_page
toc:  true
---
---
What is jekyll?/ jekyll의 디렉토리 구조/ 포스트 꾸미기/ 사진 넣기/ 표 만들기
  
  
  
## What is jekyll?
  
'jekyll'이란 github에서 개발한 또 다른 사이트 개발 툴로, 블로그 지향적인 정적 사이트 생성이 가능하다. 이에 핵심 구동 역할로서 꼽을 수 있는 것 중 하나가 텍스트 변환 엔진이라는 것인데 이는 간단히 말해 마크업 언어로 글을 작성하면 이를 미리 정의해 둔 규착에 따라 다양한 레이아웃으로 포장하여 정적 웹사이트로 만들어주는 기능을 수행한다.
  
_config.yml을 수정하면 사용자의 입맛에 맞게 블로그 기본 툴(이름, 소개, 사이트 연동 등 템플릿에 따라 그 구성이 다름)을 변경할 수 있고, _post 디렉토리에 파일을 추가하면 이를 통해 자신이 작성한 포스트를 블로그에 업로드 하여 볼 수 있다.  
  
  

## jekyll의 디렉토리 구조
  
1. _config.yml : 환경설정 정보 보관, 명령어 실행을 옵션으로 설정하지 않아도 _config.yml 파일에 정의해두면 편리하게 사용 가능
  
2. _drafts : 'draft'의 뜻은 아직 미완성 상태인 초안을 뜻 함. 파일명 형식에 날짜가 지정되지 않은 게시 전의 포스트를 보관
  
3. _includes : 재사용에 쓰이는 파일을 담는 디렉토리, 포스트 또는 레이아웃에 쉽게 코드 삽입 가능
  
4. _layouts : 포스트 사용에 쓰이는 템플릿을 담는 디렉토리, 'title'을 기준으로 각 포스트 별 레이아웃 선택이 가능
  
5. _posts : 사용자의 컨텐츠를 담는 디렉토리, 'YEAR-MONTH-DAY-TitleName.MARKUP'이라는 명명 규칙을 따라 파일을 저장해야 함
  
6. _data : 사이트에 사용할 데이터를 적절한 포맷으로 정리하여 보관하는 디렉토리
  
7. _sass : 사용자의 main.scss 에 임포트할 수 있는 Sass 조각들, 하나의 스타일시트 파일 main.css 로 가공되어 사용자의 사이트에서 사용하는 스타일들을 정의
  
8. _site : Jekyll 이 변환 작업을 마친 뒤 생성된 사이트가 저장되는 (디폴트) 경로
  
9. .jekyll-metadata : jekyll에서 해당 디렉토리를 참고하여 마지막으로 빌드된 후 한 번도 수정 과정을 거치지 않은 파일, 다음 빌드 때 어떤 파일을 생성해야 하는지 등을 판단
  
  
  
## 포스트 꾸미기 
  
포스트 글씨 설정
   
- **To bold text**, use `<strong>`.
- *To italicize text*, use `<em>`.
- <mark>To highlight</mark>, use `<mark>`.
- Abbreviations, like <abbr title="HyperText Markup Langage">HTML</abbr> should use `<abbr>`, with an optional `title` attribute for the full phrase.
- Citations, like <cite>&mdash; Mark Otto</cite>, should use `<cite>`.
- <del>Deleted</del> text should use `<del>` and <ins>inserted</ins> text should use `<ins>`.
- Superscript <sup>text</sup> uses `<sup>` and subscript <sub>text</sub> uses `<sub>`.
  


## 사진 넣기 

Step 1. assets 디렉토리에 사진 저장할 용도의 하위 디렉토리 생성하기
  
Step 2. 포스팅에 쓰일 사진들을 모두 /assets/fileName (여기서 필자는 img) 안에 넣기
  
Step 3. 포스팅 내 사진들의 링크를 다음과 같이 변경하기
  
![Sample](/assets/imge/Sample.jpg)
  
Step 4. git push 명령어를 사용한 후 확인 해보면 변경 사항 확인이 가능하며, 예시는 JPG 파일이지만 PNG, GIF도 확장자만 바꾸어 주면 사용 가능 !!
  
  
  
## 표 만들기 

| Name | Upvotes | Downvotes | Total | abstention |
|:----:|:-------:|:---------:|:-----:|:----------:|
| Haeun | 13 | 10 | 23 | 0 |
| Dayoung | 11 | 11 | 22 | 1 |
| Bohyun | 12 | 9 | 21 | 2 |
  
![Table](/assets/imge/Table.jpg)
  
위 사진처럼 문자 세 개만을 사용하여 간편하게 표를 만들 수 있다.
  
i) : 가 왼쪽에 붙으면 왼쪽 정렬  
  
ii) : 가 양쪽에 붙으면 중앙 정렬  
  
iii) : 가 오른쪽에 붙으면 오른쪽 정렬이며, 
  
일반적인 텍스트와 마찬가지로 이탤릭/ 강조 표시가 가능하며 span tag를 사용하면 글자 색 변경도 가능하다. 
  
---