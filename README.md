  ### sinnara2021/story
  =============
  # 👩🏻 신나라샘의 챗봇 제작 스토리방
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





