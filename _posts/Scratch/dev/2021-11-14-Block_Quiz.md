---
title:  "[스크래치] 블록 채우기 퀴즈 만들기"
excerpt: "작은 블록으로 화면을 다양한 애니메이션으로 채워보자"

categories:
  - Scratch_dev
tags:
  - [Scratch, Animation]

toc: true
toc_sticky: true
 
date: 2021-11-14
last_modified_at: 2021-11-14
---

# 만들 프로젝트 설명

![Animation](https://user-images.githubusercontent.com/55564114/141668320-e97e5e2c-8816-4a7c-88d2-d213ed8ac38b.gif)  

아이고.. 위에가 약간 짤렷네요...  

오늘 만들어본 프로젝트는 **작은 블록을 다양한 애니메이션**으로 화면 채우기에요.  

- 조건  
1. 🏴 을 클릭하면, 1 ~ 7 중 하나을 입력하면 그 숫자에 맞는 애니메이션 나타내기 
2. 애니메이션을 구상하기 
3. 애니메이션 구현하기

---

# 1. 디자인

## 1.1 스프라이트

![스크린샷(35)](https://user-images.githubusercontent.com/55564114/141668471-9166d6d5-dee8-42f1-949b-52aef786c21a.png)  

- Avery  

|속성|내용|상세 사항|
| :--- | --- | :---: |
|생성 방법| 스프라이트 고르기 | Avery |
|스프라이트 이름 | 변경 안함 | Avery |
|모양 | 변경 안함 | Avery-a |
| x | 변경 안함 | |
| y | 변경 안함 | | 
| 보이기 | 변경안함 | on |
|크기 | 변경안함 | 100|
|방향 | 변경안함 | 90 |

- 1 ~ 7번 블록  

|속성|내용|상세 사항|
| :--- | --- | :---: |
|생성 방법| 스프라이트 그리기 | 1.1.1 확인 |
|스프라이트 이름 | 변경 | 1~7번 |
|모양 | 선택 | 일반 |
| x | 변경 안함 | |
| y | 변경 안함 | | 
| 보이기 | 변경안함 | off |
|크기 | 변경안함 | 100|
|방향 | 변경안함 | 90 |

### 1.1.1 스프라이트 그리기

![스크린샷(37)](https://user-images.githubusercontent.com/55564114/141668644-befce6cb-3a80-4ff4-af86-3511a1deda07.png)  

![스크린샷(37) (1)](https://user-images.githubusercontent.com/55564114/141668692-66aa5d85-ac2f-4047-a60b-f5fdd2a16109.png)  

- 순서  

|순서|설명|상세 변경사항|
|:---:|---|:---:|
|1|스프라이트 그리기 클릭||
|2|"직사각형" 선택 후, 중앙에 박스 그리기 |사이즈 : 58 X 56|
|3|모양 이름 변경하기|"일반"|
|4|채우기색 변경하기| 색상 : 0 <br> 채도 : 0 <br> 명도 : 90|
|5|윤곽선 색 변경하기|색상 : 0 <br> 채도 : 0 <br> 명도 : 90 <br> 선 굵기 : 10 |  
|6| 모양 복사하기| "일반(모양)" 복사|
|7| 복사한 모양 이름 변경하기| "클릭"|
|8| 복사한 모양, 채우기색 변경하기|색상 : 0 <br> 채도 : 0 <br> 명도 : 70|
|9| 복사한 모양, 윤곽선 색 고정| 변경 x|

## 1.2 배경
- 없음.

---

# 2. 블록코딩

## 2.1 변수  

1. 블록 번호  
1.1 이 스프라이트에서만 사용  
2. 반복문 카운트  
2.1 모든 스프라이트에서만 사용  

- 설명  
1. "블록 번호(변수)"는 복제(생성)된 블록의 순서를 지정해주기 위해서 생성됨.  
2. "블록 번호(변수)"가 왜 **이 스프라이트에서만 사용**일까?  
2.1 이유 : 복제(생성)된 스프라이트가 각각의 변수를 갖게 하기 위함.  만약 **모든 스프라이트에서만 사용**이면, 모든 블록 번호가 같아짐.  
3. "반복문 카운트(변수)"는 왜 사용했을까 ?  
3.1 스크래치에서는 반복문(n번 반복하기)에서 현재 몇 번째 실행중인지 안알려줌...  
(아마 앤트리는 알려주던 걸로 기억함...)  

## 2.2 내 블록 
- 없음.  


## 2.3 스프라이트 블록코딩

 - Avery  

![스크린샷(38)](https://user-images.githubusercontent.com/55564114/141668912-0f4062e1-c728-4ea9-a718-c65250c08fc1.png)  

- 설명  
간단히 1 ~ 7 숫자만 입력 받고, 각 숫자에 맞는 신호를 보내서 애니메이션을 실행한다. 위 그림에서는 3 까지밖에 없지만, 너무 길어서 7 까지 붙여주세요.  

---

 - 1번  

![Animation](https://user-images.githubusercontent.com/55564114/141668944-f500423f-2444-43e2-8b70-dca94aa408a0.gif)  

![스크린샷(40)](https://user-images.githubusercontent.com/55564114/141668982-ec962130-d27c-497b-8a94-4f170be69730.png)  

- 2번  

![스크린샷(41)](https://user-images.githubusercontent.com/55564114/141669039-655ec80f-a255-4076-a68c-8cac15daf30d.png)  

- 3번  
- 4번  
- 5번  
- 6번  
- 7번  

- 설명  
1, 2번만 보여드리고 나머지 3 ~ 7번은 직접 만들어보세요.  
아이들을 가르치다보면 일일히 코드를 보여주면서 하는 것보다  
원리를 알려주고, 어느 부분을 수정하면 변화가 생기는지만 알려주면 그 이후에는 스스로 고민하면서 잘 하더라구여 ㅋㅋ  
오히려 스스로 생각하게 하면 더 성취도는 높아보이더라구여.  😊😊😊

---

# * 추가 설명

## 변수명 다름 

코드 보시면 **번호 = 블록 번호** 라고 생각해주시면 되요.

## 변수를 사용한 이유  

블로그를 쓰다보니까 변수를 왜 사용했는지 설명은 써놨지만, 눈으로 체크할 부분은 없어서 이미지 넣어드릴게요.  

![스크린샷(43)](https://user-images.githubusercontent.com/55564114/141669152-2a8f6a11-fdb3-48c1-8d47-fec9d0e9c840.png)  

생성된 블록을 클릭하면 색상을 변경을 해주고  
31 , 41 , 51 , 61 숫자 보이시나요?  
블록을 클릭하면 2초 동안 **블록이 몇 번째로 생성됬는지** 알게해주었어요.  
블록이 몇 번째로 생성됬는지 알게해주기 위해서 변수을 사용했어요.

---
지금 포스팅을 한지 얼마안되서 너무 어렵네요... 수업하는 거랑 차이가 커요.  🤢🤢
또한, 수업을 할 때는 아이들이 모르면 직접 가서 설명을 해주면 되는데... 온라인 수업도 코로나 때문에 해봤는데 너무 어렵더라구여  

**모르는 건 댓글 달아주시면 답변 드릴게요! 🤷**



---
