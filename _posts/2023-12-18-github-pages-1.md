---
title:  "How to use GitHub Pages(1)"
excerpt: "블로그 생성 + 첫 포스팅"

categories:
  - GitHub Pages
tags:
  - GitHub Pages
last_modified_at: 2023-12-18
---

티스토리 블로그를 몇 년 쓰다보니 커스텀이 번거롭고, 소스코드를 공유할 때 예쁘지가 않아서(가장 큰 이유) GitHub Pages를 시작해보기로 했습니다. 커스텀을 내가 원하는대로 할 수 있다는 점이 제일 기대됩니다. ㅎㅎ 시간적 여유가 될지는 모르겠지만 나중에 티스토리 블로그 글 중 괜찮은 것만 모아서 옮겨볼 생각입니다.

>지킬(Jekyll) : static websites generator로, markdown 파일을 html파일로 변환해주는 블로그 플랫폼.

static website란 어떤 웹사이트에 접속했을 때 모든 사람들에게 동일한 결과물로 보이는 웹사이트를 말합니다. GitHub Pages는 Jekyll로 만든 웹사이트를 무료로 호스팅 해주는 역할을 합니다.
<br/>

---

## 1. 테마 선택
먼저 적용할 테마를 선택합니다. 아래 링크에서 무료 테마가 많으니 이 중에서 골라보겠습니다.
<br/>

[https://jekyllthemes.io/free](https://jekyllthemes.io/free)
<br/>
위 링크에서 마음에 드는 테마를 골랐다면 다음과 같이 fork 버튼을 눌러 블로그 소스를 본인의 깃허브 계정으로 복사해옵니다.

![github-pages-1-1](https://github.com/geukggom/geukggom.github.io/assets/80306984/f1132d78-b1db-4374-ba60-cca19007e63f)
<br/>
<br/>

바로 세팅에 들어가서 [깃헙 아이디].github.io 이름으로 레포지토리 이름을 변경해줍니다. 여기서 입력한 레포지토리의 이름이 블로그의 주소가 될 예정입니다. 나중에 커스텀 도메인도 사용해보고 싶은데, 방법은 차차 알아가보도록 하겠습니다.

![github-pages-1-2](https://github.com/geukggom/geukggom.github.io/assets/80306984/0a3a16ff-c55d-4f39-a57b-756940b67594)
<br/>
<br/>

---

## 2. 간단한 블로그 세팅
레포지토리를 만들고 이름을 변경하는 것까지 완료했으면 _config.yml 이름의 파일을 찾습니다. 이 파일을 찾아 수정해줄겁니다. 이렇게 블로그의 이름과 url을 세팅해줍니다.
```
title:              GGTales
email:              geukggom@gmail.com
description:        극꼼 이야기
author:             Geukggom
baseurl:            ""
url:                "https://geukggom.github.io"
```
<br/>
수정한 다음에 커밋을 올리고, 아까 레포지토리 이름으로 설정한 geukggom.github.io 주소로 들어가보면 아까의 기본 테마에서 블로그가 수정되었음을 확인할 수 있습니다.
<br/>

![image](https://github.com/geukggom/geukggom.github.io/assets/80306984/c35468bd-e6fc-46d5-9654-8ae94d1aaebc)


생각보다 간단하게 끝났습니다!
이제 예시로 있던 글들을 지우고 첫 포스팅을 올려보겠습니다.
<br/>

---
## 3. 포스팅 업로드
레포지토리 아래에 _posts이름의 폴더에 작업해줄겁니다. 폴더가 없다면 하나 생성해주세요.
제 블로그 테마를 가져올 때 딸려온 예시 포스팅이 들어있는걸 확인할 수 있습니다. 지우고 Add file 버튼을 눌러주세요.
![github-pages-1-7](https://github.com/geukggom/geukggom.github.io/assets/80306984/6e94b3c4-2793-42a2-870a-5c351743f4cf)
<br/>
<br/>

파일 이름은  **년도-월-일-아무문자.md**  로 적어주세요. 여기에 적은  아무문자가 블로그의 url 주소가 됩니다.
<br/>
(이 포스팅의 경우 2023-12-18-github-pages-1.md 이름으로 작성되었습니다)

파일의 확장자가 md이므로 마크다운 언어로 작성해주셔야하는데요, 마크다운 언어로 작성하면 바로바로 확인할 수 없다는 점이 불편한데, 그럴때는  [에디터](https://stackedit.io/)를 사용하면 됩니다. 링크에 걸린 사이트는 제가 이 포스팅을 쓰면서 사용한 에디터인데요, 작성하면서 바로바로 확인할 수 있다는 점이 편리합니다.

<br/>

md파일을 그냥 작성해서 업로드할 경우 이렇게 입력한 url이 포스팅의 제목에 반영되고 글 내용이 어중간하게 잘려서 미리보기로 보이는 것을 볼 수 있습니다.

![image](https://github.com/geukggom/geukggom.github.io/assets/80306984/a7baaeaa-12bf-4423-b63e-5ffb22ddc3ea)
<br/>

파일을 다시 수정해서 글의 맨 앞머리에 다음 코드를 입력해주면 원하는대로 제목과 미리보기 내용이 입력됩니다.
```
---
title:  "How to use GitHub Pages(1)"
excerpt: "블로그 생성 + 첫 포스팅"

categories:
  - GitHub Pages
tags:
  - GitHub Pages
last_modified_at: 2023-12-18
---
```
<br/>

---
<br/>

![image](https://github.com/geukggom/geukggom.github.io/assets/80306984/6159cb80-ed88-400b-8899-92ff96de1226)

여기까지 깃허브 페이지스로 블로그 만드는 방법을 알아보았습니다!
쓰다보니 이 블로그에 목차, 검색, 카테고리 기능이 필요할 것 같아, 다음 포스팅에서는 이 기능들을 추가하는 방법을 알아보겠습니다.
