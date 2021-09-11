  ### sinnara2021/story
  =============
  # 👩🏻 신나라샘의 챗봇 제작 스토리방
  
  https://user-images.githubusercontent.com/79739569/132930276-0eaae252-dcd3-40b2-bbb3-f4e614c4bc3e.jpg
  -------------
   ### 챗봇삽입 default 페이지 만드는 경로
  _layouts/default.html
![image](https://user-images.githubusercontent.com/79739569/132869335-d9c5560a-0ad6-445f-ad58-91427fcf1372.png)
<hr/>

   ### 챗봇삽입 소스코드
  챗봇 삽입 소스 코드는 default.html 페이지 열어보기!
  <hr/>

  ### 여러가지 응답 만들기
  '''
  Responses
  
  Custom Payload
  
  1. Description type :  
  Intents 이름: richDes   
  Training phrases : 리치설명
  

  {
    "richContent": [
     [
       {
         "title": "전등 리스트",
         "type": "description",
         "text": [
           "안방전등",
            "거실전등"
          ]
        }
     ]
    ]
  }

2. Info type
Intents 이름:  richInfo  
Training phrases : 리치정보


{
  "richContent": [
    [
      {
        "type": "info",
        "title": "제목",
        "subtitle": "부제목",
        "image": {
          "src": {
            "rawUrl": "http://117.16.177.40/image/i2r_small.png"
          }
        },
        "actionLink":"https://i2r.link"
      }
    ]
  ]
}

3. Image type
Intents 이름:  richImage 
Training phrases : 리치그림


{
  "richContent": [
    [
      {
        "type": "image",
        "accessibilityText":"MBD Image",
        "rawUrl": "http://117.16.177.40/image/sunset.jpg"
      }
    ]
  ]
}

4. Button type
Intents 이름:  richButton 
Training phrases : 리치버튼


{
  "richContent": [
    [
      {
        "link":"https://sinnara2021.github.io/chatbot/",
        "text": "Go to Idea to Real",
        "icon": {
          "type":"link",
          "color":"#FF9800"
        },
        "type": "button"
      }
    ]
  ]
}

5. Suggestion Chips
Intents 이름:  richSuggestion  
Training phrases : 리치선택

{
  "richContent": [
    [
      {
        "type":"chips",
        "options": [
          {
            "text":"yes"
          },
          {
            "text":"no"
          }
        ]
      }
    ]
  ]
}

6. List Response Type
Intents 이름:  richList 
Training phrases : 리치리스트

{
  "richContent": [
    [
      {
        "title":"List item 1 title",
        "subtitle":"List Item 1 subtitle",
        "type":"list",
        "event": {
          "parameters":{},
          "name":"WELCOME",
          "languageCode":"en"
        }
      },
      {
        "type":"divider"
      },
      {
        "title":"List item 2 title",
        "subtitle":"List Item 2 subtitle",
        "type":"list",
        "event": {
          "parameters":{},
          "name":"PARALLEL",
          "languageCode":"en"
        }
      }
    ]
  ]
}



'''
<hr/>
### 마크다운 문법 알아보기

https://www.dropbox.com/s/mzp9tq4qtfjdlif/20141021_markdown_use_tip.md?dl=0


# 제목 1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6
![image](https://user-images.githubusercontent.com/79739569/132870001-c4b88bfd-9b9e-4b67-bfed-043fea45a258.png)


![image](https://user-images.githubusercontent.com/79739569/132870090-11936485-fcde-42c5-a8d2-2264f2234c86.png)
이텔릭체는 *별표(asterisks)* 혹은 _언더바(underscore)_를 사용하세요. 
두껍게는 **별표(asterisks)** 혹은 __언더바(underscore)__를 사용하세요.
**_이텔릭체_와 두껍게**를 같이 사용할 수 있습니다. 
취소선은 ~~물결표시(tilde)~~를 사용하세요. 
<u>밑줄</u>은 `<u></u>`를 사용하세요.
![image](https://user-images.githubusercontent.com/79739569/132870103-7018344a-c460-4348-ab27-3a2087db44e2.png)


[임호고챗봇제작 깃헙페이지](https://yunsugyoung.github.io/talk/) 
![Image](https://cdn.pixabay.com/photo/2017/06/10/07/21/chat-2389223__340.png)
![image](https://user-images.githubusercontent.com/79739569/132870129-bae6b843-b869-42d0-b655-bacd2650b6fb.png)


- - -
(Hyphens)
* * *
(Asterisks)
_ _ _
(Underscores)
![image](https://user-images.githubusercontent.com/79739569/132870150-e026b638-ff94-42c2-b9ea-d0dbd05318fb.png)

| 값 | 의미 | 기본값 |
|---|:---:|---:|
| `static` | 유형(기준) 없음 / 배치 불가능 | `static` |
| `relative` | 요소 자신을 기준으로 배치 |  |
| `absolute` | 위치 상 부모(조상)요소를 기준으로 배치 |  |
| `fixed` | 브라우저 창을 기준으로 배치 |  |
![image](https://user-images.githubusercontent.com/79739569/132870166-0c3659b6-3632-48ce-9fff-c72e8c25aeb8.png)

![image](https://user-images.githubusercontent.com/79739569/132870206-ac78a972-7076-4d3f-ab36-bdbf2f3f9fed.png)
