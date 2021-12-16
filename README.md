# It's My Github Blog !!  
## 깃허브 페이지를 이용하여 만든 깃허브 블로그  
![my blog](https://user-images.githubusercontent.com/81706832/146318816-a67c6df5-a727-4e7d-888f-d8c7664da1d2.jpg)
  
  
---
## Build 과정   
Step 1. Git을 먼저 설치하고, Github 계정이 없다면 이를 생성한 후  
나의 깃허브 계정에 username.github.io 라는 이름의 레파지토리 생성하기
  
Step 2. 'clone' 명령어를 이용하여 원격저장소의 레파지토리를 로컬저장소에 복제하기  
  
Step 3. https://rubyinstaller.org/downloads/  
위 페이지에서 사용자의 운영체제에 맞는 루비 + 개발자킷 설치 프로그램 다운,  
이 과정이 끝나면 Start Command Prompt with Ruby 실행하기  
  
- 'gem inatall jekyll bundler' 명령어를 통해 패키지 설치  
- 'jekyll -v' 명령어를 통해 jekyll 설치 여부 확인  
- 'jekyll new .' 명령어를 통해 현재 디렉토리 내에 블로그 파일 생성  
- 'jekyll serve' 명령어를 통해 지킬 실행  
  
Step 3. http://jekyllthemes.org/ https://jekyllthemes.io/free  
위 사이트를 참고하여 적용하고 싶은 테마를 Download/ fork 등의 방법을 통해 가져온 후,  
터미널을 이용하여 가져온 테마를 Step 1 에서 생성한 나의 원격저장소에 add > commit > push 하기  
  
Step 4. '_config.yml', 'navigation', 'social'에서 title, description 등의 적절한 수정 과정 거치기  
  
Step 5. 작성한 포스트 파일은 '_posts' 폴더에 넣어주기  
(여기서 유의할 점은 각 게시글의 layout을 post로 설정해주어야 함)  
  
Step 6. 작성한 포스트 파일의 사진들은 Markdown 형식의 주소가 필요한데,  
자세한 내용은 [여기의](https://gyuwonsong.github.io/july22.github.io/2021/12/10/What-is-jekyll/) '사진넣기'를 참고  
  
Step 7. 하나 뿐인 나만의 블로그 만들기, 끝 :) !!!!!  

---
