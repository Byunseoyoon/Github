# **Markdown Basic A to Z**
```
20201852 변서윤
```
___
<!-- Heading -->
## **1. Heading**
___
`#`, `=`, `-` 를 사용하여 header를 작성할 수 있다.
|level|작성방법|
|:--:|:--:|
|1단계|# heading| 
|2단계|## heading|
|3단계|### heading|
|4단계|#### heading|
|5단계|##### heading|
|6단계|###### heading|
|
- ***example***
># heading (1단계) 
>## heading (2단계) 
>### heading (3단계)
>#### heading (4단계)
>##### heading (5단계)
>###### heading (6단계)

- ***`warning`***

>|right|wrong|
>|:--:|:--:|
>|# heading| #heading|

>`'#', 'heading'`사이 **공백**이 있어야 한다.

<br>

 ## **1.1 # heading 대체 문법**
|level|작성방법|
|:--:|:--:|
|1단계|heading<br/>=======|
|2단계|heading<br/>-------|
|
- ***example***
>heading (1단계 '=')
>=======
>heading (2단계 '-')
>------- 
<br>

___
<!-- Paragraphs -->
## **2. Paragraphs / 문단**
___
- **방법**
```
  단락 만들기는

    (공백줄) 

  공백을 사용하면 된다.
```
- ***example***

>  단락을 만들기 위해서는
> 
> 공백을 사용하면 된다.

- ***`(warning)` wrong way***
>***example***
>
>(띄어쓰기)markdown은 1번 초과된 띄어쓰기를 무시하기 때문에
>
>(띄어쓰기)Paragraphs을 만든다고 첫줄에 띄어쓰기를 하면 적용이 안된다. 

>**output**
>
>  markdown은 1번이 넘는 띄어쓰기를 무시하기 때문에
>
>  Paragraphs을 만든다고 첫줄에 띄어쓰기를 하면 적용이 안된다. 

<br>

___
<!-- Line breaks-->
## **3. Line breaks / 개행**
___ 
  **`<br>`** 또는 **`\`** 을 사용하면 개행을 할 수 있다.  
|종류|작성방법|
|:--:|:--|
|`<br>`|br로\<br>개행하기\<br><br>개행| 
|`\`|역슬래쉬로 \\ <br> 개행하기\\ <br>개행|
|
- ***example***
>br로<br> 개행하기<br>
개행

>역슬래쉬로\
개행하기

*참고 : `'\'`는 사용을 권장하지 않음.*

<br>

___
<!-- Emphasis -->
## **4. Emphasis / 강조**
___ 
`'*', '_'`를 이용하여 강조할 수 있다.
## **4.1 Bold**
|종류|작성방법|example|
|:--|:--|:--|
|`** **`|I use \*\*star**| I use **star**|
|`__ __`|I use \_\_under bar__|I use __under bar__|
|

>  *`'__ __'` 사용은 권장하지 않음* 

<br>

## **4.2 Italic**
|종류|작성방법|example|
|:--:|:--|:--|
|`* *`|I use \*star*| I use *star*|
|`_ _`|I use \_under bar_|I use _under bar_|
|

>   *`'__ __'` 사용은 권장하지 않음* 


<br>

## **4.3 Bold and Italic**
|종류|작성방법|example|
|:--:|:--|:--|
|`*** ***`|I use \*\*\*star***| I use ***star***|
|`___ ___`|I use \_\_\_under bar___|I use ___under bar___|
|`__* *__`|I can use \_\_\*all*__|I use __*all*__|
|`**_ _**`|I can use \*\*\_all_**|I use **_all_**|
|

>   *`'___ ___'` 사용은 권장하지 않음* 

<br>

___
<!--  Blockquotes -->
## **5. Blockquotes / 인용구**
___ 
`'>'`기호를 사용하여 인용구를 만들 수 있다.
  
- **작성방법**
```
> 초밥 먹고 싶다.
```
- ***example***
> 초밥 먹고 싶다.<br>

<br>

## **5.1 인용구 한 단락으로 만들기**
- **작성방법**
```
> 새우초밥
>
> 연어초밥
```
- ***example***
> 새우초밥
> 
> 연어초밥<br>

<br>

## **5.2 인용구 중첩하기**
- **작성방법**
```
> I love sushi
>> but I hate raw fish
```
- ***example***
> I love sushi
>>but I hate raw fish<br>

<br>

## **5.3 인용구에 다른 요소 사용하기**
- **작성방법**
```
> ## 철이 없었죠
> - 커피가 좋아서
>
> *유학*을 했다는 **자체가**
```
- ***example***
> ## 철이 없었죠
> - 커피가 좋아서
> 
> *유학*을 했다는 **자체가**

<br>


___
<!-- List -->
## **6. List**
___ 
## **6.1 Number List**
- **작성방법**
```
1. 순두부찌개
2. 부대찌개
3. 김치찌개
(탭)   1. 돼지고기
(탭)   2. 참치
```
- ***example***
>1. 순두부찌개
>2. 부대찌개
>3. 김치찌개
>     1. 돼지고기
>    2. 참치
<br>

<br>

**` + list의 시작숫자가 1이면 그 다음숫자는 순서대로 작성하지 않아도 된다.`**

```
1. 로제떡볶이
6. 로제찜닭
3. 로제파스타
```
- ***example***
>1. 로제떡볶이
>6. 로제찜닭
>3. 로제파스타<br> 

*참고 : '1)' 의 사용은 권장하지 않음.*

<br>

## **6.2 Symbol List**
`'*', '-', '+'` 를 사용하여 list를 만들 수 있다.
|종류|작성방법|
|:--:|:--|
|**`*`**|* First<br> * Second<br> * Third|
|**`-`**|- First<br> - Second<br> - Third|
|**`+`**|+ First<br> + Second<br> + Third|
|
- ***example***
>* First
>* Second
>* Third<br> 

세가지 기호의 결과는 위의 모양으로 모두 같다.<br>
Number List와 같이 들여쓰기도 가능하다.
> - First
>   - First
>   - seond
> - Second

*참고 : 세가지 기호를 섞어서 쓰는 건 권장하지 않음.* 

<br>

## **6.3 List에 다른 요소 더하기**
6.3.1 문장 끼워 넣기
- **작성방법**
```
- 첫번째
- 두번째
무 야 호 !
- 세번째 
```
- ***example***
>- 첫번째
>- 두번째
>
>   무 야 호 !
>
>- 세번째 

<br>

6.3.2 인용구 끼워넣기
- **작성방법**
```
- 첫번째
- 두번째
> 무 야 호 !
- 세번째 
```
- ***example***
>- 첫번째
>- 두번째
> > 무 야 호 !
>- 세번째 

<br>

6.3.3 블럭코드 끼워넣기
- **작성방법**
```
1. First
2. Sesond
(탭 두 번 or space 8번)    안녕
(탭 두 번 or space 8번)       HI  
3. Third
```
- ***example***
 1. First
 2. Second
          
         안녕
            HI

3. Third<br>

<br>

6.3.4 사진 끼워넣기
- **작성방법**
```
1. 숭실대 로고가 있는 파일 열기
2. 마블

      ![ssu logo](ssu.jpg)

3. 파일 닫기
```
- ***example***
1. 숭실대 로고가 있는 파일 열기
2. 숭실대

      ![ssu logo](ssu.jpg)

3. 파일 닫기

<br>

6.3.5 리스트 끼워넣기
- **작성방법**
```
1. First
1. Second
     - one
     - two
3. Third
```
- ***example***
>1. First
>1. Second
>     - one
>     - two
>3. Third

<br>

___
<!-- Code -->
## **7. Code**
___ 
``억음 부호(`)``를 사용하여 단어나 어구를 코드로 표시 할 수있다. 

## **7.1 단어 코드 표시하기**

|설명|작성방법|example|
|--|:--|--|
|단어를 표시할 때|\`코드\` 표시하기|`코드` 표시하기|
|(`)억음부호를 직접 사용할 때|\`\`코드 \`표시\`하기``|``코드 `표시`하기``|
|

<br>

## **7.2 코드블럭 만들기**
- **작성방법**


(탭 두 번 or space 8번)       HI
- ***example***
          
      HI
- **작성방법**

    **\`\`\`**

  안녕

  **\`\`\`**
- ***example***
  ```
  안녕
  ```
<br>

___
<!-- Horizontal Rules -->
## **8. Horizontal Rules**
___ 
`*, -, _` 를 사용하여 경계선을 만들 수 있다.

- **작성방법**
```
`*, -, _`를  

***

각 3개 이상 써주개 되면

---

경계선이 생긴다

___
```
- ***example***

>`*, -, _`를   
>***
>각각 3개 이상 써주게 되면
>
>---
>
>경계선이 생긴다
>___

*`warning` : 경계선을 쓸 때 이전 line에 blank lines을 만들어야 한다.* 

<br>

___
<!-- Links -->
## **9. Links**
___
`[], <>` 를 이용하여 링크를 표시할 수 있다.

## **9.1 링크 표시하기**
|종류|작성방법|example|
|--|:--|--|
|\[Title\](주소)|\[Google](https://www.google.com/)|[Google](https://www.google.com/)|
| \<URL> | \<https://www.google.com>|https://www.google.com|
| <Email 주소>|\<bsy4943@naver.com>|<bsy4943@naver.com>|
|

*참고 : `*, _`를 사용하여 링크를 **bold** 또는 Italic으로 나타낼 수 있음.*

<br>

## **9.2 외부 참조 링크**
- **작성방법**
```
왼쪽 대괄호 안에 제목, 오른쪽엔 숫자를 쓰고
[Markdown][1]

[1]: <https://www.markdownguide.org/>
숫자로 시작하는 외부 주소를 적는다
```
- ***example***

> 왼쪽 대괄호 안에 제목, 오른쪽엔 숫자를 쓰고<br>
> [Markdown][1]
>
>[1]: <https://www.markdownguide.org/>
>숫자로 시작하는 외부 주소를 적는다

<br>

*`참고 `: 이중 따옴표, 단일 따옴표 또는 괄호를 이용해 링크의 제목을 붙일 수 있다.<br>*
```
ex) [1]: https://www.markdownguide.org/ "Markdown"
    [1]: https://www.markdownguide.org/ (Markdown)
    [1]: <https://www.markdownguide.org/> 'Markdown'
```
*`참고 `: 호환성을 위해 URL이 .%20으로 공백을 인코딩하도록 한다.<br>*
```
ex) [link](https://www.example.com/my great page)
    [link](https://www.example.com/my%20great%20page) (<-great!)
```
<br>

___
<!-- Images -->
## **10. Images**
___
## **10.1 Add images**
- **작성방법**

 ![제목](이미지 경로) <br>
 ```
 ![짱구](hard.jpg)
 ```
- ***example***

  ![짱구](hard.jpg)

<br>

## **10.2 Linking images**
- **작성방법**

\[![제목](이미지 경로)](웹사이트 Link)
```
[![NASA](NASA.jpg)](https://www.nasa.gov/)
```
- ***example***
  
  [![NASA](NASA.jpg)](https://www.nasa.gov/)

<br>

___
<!-- Escaping Characters -->
## **11. Escaping Characters**
___
markdown에서 \#, \*, \-, \<> 등과 같이 정해진 역할이 있어서 그 자체로는 화면에 표시할 수 없는 문자들은 그 앞에 `\`를 붙여서 표시한다.
- **작성방법**
  ```
  \#, \*, \-, \<>
  ```
- ***example***
  >  \#, \*, \-, \<>

  <br>

___
<!-- HTML -->
## **12. HTML**
___
markdown에서는 html 문법을 사용할 수 있게 해놓았다.

- **작성방법(예시)**
  ```
  This <strong>word</strong> is bold. This <em>word</em> is italic.
  ```
- ***example***
  >This <strong>word</strong> is bold. This <em>word</em> is italic.

<br>
<br>
<br>

# Github Flavered Markdown(GFM)

 GFM의 표준 Markdown에 대한 확장 부분의 사용법
 click [here](https://github.com/Byunseoyoon/README)

> 링크 주소: https://github.com/Byunseoyoon/README

