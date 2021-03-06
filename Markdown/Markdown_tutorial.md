# 마크다운<sup>Markdown</sup> 튜토리얼

# 목차

- [마크다운<sup>Markdown</sup>이란?](#마크다운markdown이란)
- [마크업 문법<sup>Markup Syntax</sup>](#마크업-문법markup-syntax)
  - [헤더<sup>Header</sup>](#헤더header)
  - [강조<sup>Emphasis</sup>](#강조emphasis)
  - [수평선<sup>Horizontal Rules</sup>](#수평선horizontal-rules)
  - [링크<sup>Links</sup>](#링크links)
  - [이미지<sup>Images</sup>](#이미지images)
  - [인용<sup>Blockquotes</sup>](#인용blockquotes)
  - [첨자<sup>Script</sup>](#첨자script)
  - [코드<sup>Code</sup>](#코드code)
  - [테이블<sup>Tables</sup>](#테이블tables)
  - [목차<sup>Table of Content</sup>](#목차table-of-content)
  - [요약<sup>Summary</sub>](#요약supsummarysub)
  - [각주<sup>Footnote</sup>](#각주footnote)
  - [이스케이프<sup>Backslash Escapes</sup>](#이스케이프backslash-escapes)
  - [취소선<sup>Strikethrough</sup>](#취소선strikethrough)
  - [이모티콘<sup>Emoji</sup>](#이모티콘emoji)
  - [개행<sup>Line alignment</sup>](#개행line-alignment)
  - [단락<sup>Paragraph</sup>](#단락paragraph)
  



# 마크다운<sup>Markdown</sup>이란?


마크다운(markdown)은 2004년에 존 그루버와 에런 스워츠의 협업을 통해 만들어진 일반 텍스트 기반의 경량 마크업 언어이다.

> #### 마크업 언어<sup>Markup Language</sup>란?
> 태그 등을 이용하여 문서나 데이터의 구조를 명기하는 언어

# 마크업 문법<sup>Markup Syntax</sup>

## 헤더<sup>Header</sup></div>
- h1 : 큰 제목, 문서 제목 
  
  ```
  # This is an <h1> tag
  ```
  # This is an `<h1>` tag

  ```
  This is an <h1> tag
  ===
  ```
  
  This is an `<h1>` tag
  ===

- h2 : 중간 제목, 부 제목
  
  ```
  ## This is an <h2> tag
  ```
  
  ## This is an `<h2>` tag

  ```
  This is an <h2> tag
  ---
  ```

  
  This is an `<h2>` tag
  ---
- h3 ~ h6 : 소 제목    

  ```
  ### This is an <h3> tag
  #### This is an <h4> tag
  ##### This is an <h5> tag
  ###### This is an <h6> tag
  ```
  
  ### This is an `<h3>` tag
  #### This is an `<h4>` tag
  ##### This is an `<h5>` tag
  ###### This is an `<h6>` tag

## 강조<sup>Emphasis</sup>
- ### 볼드체<sup>bold</sup>
    
  ```
  **This text will be bold**
  __This will also be bold__
  ```
  
  **This text will be bold**  
  __This will also be bold__
  
- #### 이탤릭체<sup>italic</sup>
   
  ```
  *This text will be italic*
  _This will also be italic_
  ```
  
  *This text will be italic*  
  _This will also be italic_


## 수평선<sup>Horizontal Rules</sup>
   `-`, `*` 또는 `_`를 3개 이상 입력    
  
  ```
  ---
  ***
  ___
  ``` 
  
  ---
  ***
  ___

## 링크<sup>links</sup>
- ### URL links
  URL 입력시 자동적으로<sup>Automaticl</sup> 하이퍼링크 등록    
  
  ```
  <http://github.com/>
  ```

  
  <http://github.com/>

- ### Inline links
  문구에 하이퍼링크 등록  
  
  ```
  [깃 허브](http://github.com/ "Github")
  ```
  
  [깃 허브](http://github.com/ "Github")

- ### 참조 링크
  문서 내에 같은 주소의 하이퍼링크를 효율적으로 작성할 수 있음
  참조되어지는 행과 참조할 정보를 기록하는 행은 한 행 이상의 거리가 필요
  
  ```
  [깃 허브][1]는 최고의 협업 사이트입니다.
  [깃 허브][github]를 경험해보고 싶다면 [이 곳][1]을 클릭해주세요.

  [1]:http://github.com/ "Github"
  [github]:http://github.com/ "Github"
  ```
  
  [깃 허브][1]는 최고의 협업 사이트입니다.  
  [깃 허브][github]를 경험해보고 싶다면 [이 곳][1]을 클릭해주세요.  

  [1]:http://github.com/ "Github"
  [github]:http://github.com/ "Github"

## 리스트<sup>Lists</sup>

- ### 순서가 있는 리스트<sup>Ordered Lists</sup>  
  적힌 숫자와 상관없이 순서대로 번호가 매겨진다.  
  
  ```
  1. item 1
  1. item 2
  1. item 3
    1. item 3a
    1. item 3b
  ```
   
  
  1. item 1
  1. item 2
  1. item 3  
      1. item 3a
      1. item 3b

- ### 순서가 없는 리스트<sup>Unordered Lists</sup>
  
  ```
  - item 1
    - item 1-1
      - item 1-1-1
  * item 2
    * item 2-1
      *item 2-1-1
  + item 3
    + item 3-1
      + item 3-1-1
  ```
  
  
  - item 1
    - item 1-1
      - item 1-1-1
  * item 2
    * item 2-1
      * item 2-1-1
  + item 3
    + item 3-1
      + item 3-1-1

## 이미지<sup>Images</sup>

- ### Link image
  이미지 오른쪽 마우스 클릭 -> 이미지 주소 복사 -> URL 입력
  
  ```
  ![Bird](https://cdn.pixabay.com/photo/2021/06/27/17/50/redstart-6369564__480.jpg)
  ```
  
  
  ![Bird](https://cdn.pixabay.com/photo/2021/06/27/17/50/redstart-6369564__480.jpg)

- ### Inline image  
  로컬 저장소의 경로를 입력    
  
  ```
  ![Squirrel](./image/squirrel.webp "다람쥐")
  ```
  
  ![Squirrel](./image/squirrel.webp "다람쥐")

- ### Image link  
  Combination of Image and Link    
  
  ```
  [![Squirrel](./image/squirrel.webp)](http://github.com)
  ```
  
  
  [![Squirrel](./image/squirrel.webp)](http://github.com)
  
- ### 이미지 크기 조절
  
  ```
  <img src="./image/squirrel.webp" width="150px" height="100px" title="고정 크기 설정" alt="다람쥐"></img>
  
  <img src="./image/squirrel.webp" width="40%" height="30%" title="가변 크기 설정" alt="다람쥐"></img>
  ```
   
  
  <img src="./image/squirrel.webp" width="150px" height="100px" title="고정 크기 설정" alt="다람쥐"></img>
  
  <img src="./image/squirrel.webp" width="40%" height="30%" title="가변 크기 설정" alt="다람쥐"></img>
  
## 인용<sup>Blockquotes</sup>
  
  ```
  As Kanye West said:

  > We're living the future so
  > the present is our past.
  ```
  
  
  As Kanye West said:

  > We're living the future so  
  > the present is our past.

## 첨자<sup>Script</sup>

- ### 위첨자<sup>Superscript</sup>

  ```
  문구<sup>윗첨자</sup>
  ```
  
  
  문구<sup>윗첨자</sup>

- ### 아래첨자<sub>Subscript</sub>
  
  ```
  문구<sub>아랫첨자</sub>
  ```
  
  문구<sub>아랫첨자</sub>

## 코드<sup>Code</sup>

- ### Inline code
  
  ```
  I think you should use an  
  `<addr>` element here instead.
  ```
  I think you should use an  
  `<addr>` element here instead.

- ### 펜스<sup>Fences</sup>
  * \`\`\` 펜스
  
    ~~~
    ```
    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }
    ```
    ~~~
    
    
    ```
    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }
    ```
  * \~\~\~ 펜스
    ```
    ~~~
    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }
    ~~~
    ```  
    
    ~~~
    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }
    ~~~
    
  ※ 펜스 내에 \`\`\`을 적고 싶으면 \~\~\~ 펜스를 사용, 반대도 가능

- ### 문법 강조<sup>Syntax highlighting</sup>
  
  ~~~
  ``` javascript
  function fancyAlert(arg) {
    if(arg) {
      $.facebox({div:'#foo'})
    }
  }
  ```
  ~~~
  
  
  ``` javascript
  function fancyAlert(arg) {
    if(arg) {
      $.facebox({div:'#foo'})
    }
  }
  ```

- ### 들여쓰기 코드<sup>Indented Code</sup>
  
  **조건**
  1. 띄어쓰기 4번 혹은 Tab 2번
  2. 코드와 텍스트 사이에 1행 이상의 간격이 필요  
    

  ```
      function fancyAlert(arg) {
        if(arg) {
          $.facebox({div:'#foo'})
        }
      }
  ```
  
  
      function fancyAlert(arg) {
        if(arg) {
          $.facebox({div:'#foo'})
        }
      }
      
## 테이블<sup>Tables</sup>
  - ### 테이블 생성
    
    
    ```
    Header 1 | Header 2
    -------- | --------
    Content 1 | Content 2
    Content 3 | Content 4
    ```
    
    
    Header 1 | Header 2
    -------- | --------
    Content 1 | Content 2
    Content 3 | Content 4
  
  - ### 테이블 정렬
    
    ```
    |   Left    |  Center   |   Right   |
    |:----------|:---------:|----------:|
    | 1 | 2 | 3 |
    | 4 | 5 | 6 |
    ```
    
    |   Left    |  Center   |   Right   |
    |:----------|:---------:|----------:|
    | 1 | 2 | 3 |
    | 4 | 5 | 6 |

## 목차<sup>Table of Content</sup>

  - ### 참조되어질 내용

    ```
    ##### 제 목!<sup>1</sup>
    <div id="아이디">제 목!<sup>2</sup></div>
    ```

    ##### 제 목!<sup>1</sup>

    <div id="아이디">제 목!<sup>2</sup></div>
  - ### 제목<sup>Header</sup> 참조
    
    **조건**  
    
    1. 특수 문자 (ex. ., <, /, ?, etc)와 tag (ex. `<div>`, `<sup>`, etc)는 무시
    2. 띄어쓰기는 `-`로 작성  
    3. 영어는 소문자만
    4. Header의 #개수와 상관없이 링크의 #개수는 1개
    5. #이 들어간 Header와 이름이 같으면서 위의 조건을 충족해야 함
    
    ```
    [제 목!<sup>1</sup>](#제-목1)
    ```
    
    [제 목!<sup>1</sup>](#제-목1)

  - ### ID 참조
    
    ```
    [제 목!<sup>2</sup>](#아이디)
    ```
  
    
    [제 목!<sup>2</sup>](#아이디)
    
      
## 각주<sup>Footnote</sup>
  Github는 [^id] 각주 기능을 지원하지 않기 때문에 HTML 방식을 사용
  
  ```
  각주<sup>[1](#footnotes)</sup>
  
  <a name="footnotes">1</a>: 본문에 대하는 참조 문헌이나 본문의 낱말, 문장 등의 뜻을 알기 쉽게 풀이하는 덧붙이는 글
  ```
  
  각주<sup>[1](#footnotes)</sup>
    
  <a name="footnotes">1</a>: 본문에 대하는 참조 문헌이나 본문의 낱말, 문장 등의 뜻을 알기 쉽게 풀이하는 덧붙이는 글
    
## 요약<sup>Summary</sub>
  
  ```
  <details><summary>Click</summary>
  요약 내용</details>
  ```
  
  <details><summary>Click</summary>
  요약 내용</details>

## 이스케이프<sup>Backslash Escapes</sup>
  *, _, \`와 같이 문법에 사용되는 문자 사용
  
  ```
  \*이텔리체\*
  \_\_볼드체\_\_
  \`\`\`
  ```
  
  \*이텔리체\*
  \_\_볼드체\_\_
  \`\`\`
  
## 취소선<sup>Strikethrough</sup>
  ```
  ~~취소할래요~~
  ```
  ~~취소할래요~~

## 이모티콘<sup>Emoji</sup>
  더 많은 이모티콘을 알고 싶다면 [이 곳](https://github.com/markdown-it/markdown-it-emoji/blob/master/lib/data/full.json)을 이용해주세요.
  
  ```
  :tada: :100:
  ```  
  :tada: :100:
  
## 개행<sup>Line alignment</sup>
  개행하고 싶은 문장들 사이에 띄어쓰기 2회 입력
  ```
  개행이 안될거에요.
  왜냐하면 띄어쓰기를 안했으니까요
  
  개행이 될거예요.  
  왜냐하면 띄어쓰기를 두 번 했어요
  ```
  
  개행이 안될거에요.
  왜냐하면 띄어쓰기를 안했으니까요.
  
  개행이 될거예요.  
  왜냐하면 띄어쓰기를 두 번 했어요.
  
## 단락<sup>Paragraph</sup>
  
  **방법**
  1. 단락을 나누고 싶은 곳에 두 번 Enter을 입력
  2. 단락을 나누고 싶은 곳에 `</br>`을 입력
  
  ```
  단락1
  단락2
  
  단락3</br>
  단락4  
  ```
  
  단락1
  단락2
  
  단락3</br>
  단락4  

  
    
    
