


# GOOGLE 작성 규칙


1. 선언(속성) 순서
    * 알파벳 순서대로 속성을 선언한다.
    * vendor-prefix 선언은 알파벳 선언순서를 무시한다.
    * 단, 접두어가 붙지 않는 속성을 가장 마지막에 선언한다.
    ```
    .sample {
    background-color:#000;
    border:1px solid #eee;
    -moz-border-radius:3px;
    -webkit-border-radius:3px;
    border-radius:3px;
    color:#222;
    text-align:center;
    }
    ```
2. 블록 내 내용 들여쓰기
    * 모든 블록 내부에서 들여쓰기를 한다.<br>
    ```
    .sample {
    background-color:#000;
    border:1px solid #eee;
    }
    @media screen {
            .sample {
            background-color:#222;
            border:1px solid #444;
        }
    }
    ```

3. 선언 중지
    * 마지막 속성에는 세미콜론을 제외해도 무방하지만 일관성 유지와 확장성을 위하여 모든 속성선언 끝에는 세미콜론을 붙인다.
    ```
    /* 비추천 */
    .sample {
        background-color:#000;
        border:1px solid #eee
    }

    /* 추천 */
    .sample {
        background-color:#000;
        border:1px solid #eee;
    }
    ```

4. 속성이름 뒤 여백
    * 속성과 값 사이에 한칸의 여백을 둔다.
    
    ```
    /* 비추천 */
    .sample {
        background-color:#000;
        border:1px solid #eee;
    }

    /* 추천 */
    .sample {
        background-color: #000;
        border: 1px solid #eee;
    }
    ```
5. 선언 블록 분리
    * 선택자와 속성 선언 블록 사이에 공백을 사용한다.
    * 선택자가 여럿일 경우 각 선택자 간 줄바꿈 하여 구분한다.
    ```
    .sample,
    .sample2,
    .sample3 {
        ...
    }
    ```
6. 선언 블록 분리
    * 선택자와 속성 선언 블록 사이에 공백을 사용한다.
    * 선택자가 여럿일 경우 각 선택자 간 줄바꿈 하여 구분한다.
    ```
    .sample,
    .sample2,
    .sample3 {
        ...
    }
    ```

7. 규칙(속성) 분리
    * 속성 선언이 끝나면 새로운 속성을 선언하기 전 줄바꿈 처리 한다.
    ```
    .sample {
    background-color:#222;
    color:#333;
    font-size:15px;
    }
    ```

8. 따옴표 사용
    * 알속성 값에 따옴표를 사용해야하는 경우 큰따옴표(" ")대신 작은 따옴표(' ')를 사용한다.
    * background속성의 url값에는 따옴표를 사용하지 않는다.
    * @charset 규칙을 사용할때는 큰 따옴표를 사용한다. (작은 따옴표 허용되지 않음)
    ```
    /* 비추천 */
    @import url('https://wwww.google.com/css/maia.css');
    .sample {
        font-faimy: "open sans", arial, sans-serif;
    }

    /* 추천 */
    @import url(https://wwww.google.com/css/maia.css);
    .sample {
        font-family: 'open sans', arial, sans-serif;
    }
    ```

출처 : https://code-study.tistory.com/18

<br>
<br>
<br>
<br>

# NHN 작성 규칙

| 순서 |       속성(그룹)       |  의미  |                                                관련 속성                                               |
|:----:|:----------------------:|:------:|:------------------------------------------------------------------------------------------------------:|
|   1  |         display        |  표시  |                                               visibility                                               |
|   2  |        overflow        |  넘침  |                                                    -                                                   |
|   3  |          float         |  흐름  |                                                  clear                                                 |
|   4  |        position        |  위치  |                                                    -                                                   |
|   5  |         z-index        |  정렬  |                                    top, right, left, bottom, z-index                                   |
|   6  |     width & height     |  크기  |                                                    -                                                   |
|   7  | margin & padding(그룹) |  간격  |                                                    -                                                   |
|   8  |      border(그룹)      | 테두리 |                                                                                                        |
|   9  |    background(그룹)    |  배경  |                                                                                                        |
|  10  |       font(그룹)       |  폰트  |     color, letter-spacing, text-align, text-decoration, text-indent, vertical-align, white-space등     |
|  11  |        etc(기타)       |        | 위에 언급되지 않은 나머지 속성들로 폰트의 관련 속성 이후에 선언하며, 기타 속성 내의 선언 순서는 무관함 |
---

1. 기본 규칙
    * 모든 속성은 영문 소문자로만 작성한다.
    * 따옴표 사용 범위 : 공백이 포함된 폰트명, 한글 폰트명, 문자열 데이터 타입, filter 속성의 파라미터값은 작은따옴표(' ')로 감싸며, @charset 선언 시에는 속성 값을 큰따옴표(" ")로 감싼다. 그 외의 경우에는 따옴표를 사용하지 않는다.

    * 단, 접두어가 붙지 않는 속성을 가장 마지막에 선언한다.
    * 마지막 속성의 세미콜론(;)은 삭제한다.

2. 들여쓰기
    * CSS 코드를 작성할 때는 들여쓰기를 하지 않는다.단, 중괄호”{}”가 중첩되는 경우 예외
   
3. 공백
    * 선택자 간 공백 제거 : 쉼표로 구분되는 선택자 간 공백은 제거한다.
    ```
    잘못된 예) a:hover, a:active, a:focus{textdecoration:underline}
    올바른 예)  a:hover,a:active,a:focus{text-decoration:underline}
    ```
    * 속성 간 공백 제거 : 속성 간 공백 및 속성 값 사이 공백은 제거한다.
    ```
    잘못된 예).class p{color:#000; line-height:18px}
    올바른 예).class p{color:#000;line-height:18px}
    ```
    * 중괄호 좌우 공백 제거 : 중괄호 좌, 우 공백은 제거한다.
    ```
    잘못된 예).class p {color:#000}
    올바른 예).class p{color:#000}
    ```
4. 빈 줄
    * 의미 있는 객체를 구분하기 위하여 코드 그룹 간 1줄씩 빈 줄을 넣을 수 있다.
    ```
    /* 의미 있는 그룹 1 */
    .class1{border:1px solid #000}
    .class1 img{border:1px solid #000}
            빈 줄
    /* 의미 있는 그룹 2 */
    .class2{border:1px solid #000}
    .class2 img{border:1px solid #000}
    ```
5. 선택자


<br>
<br>
<br>
<br>

# DAUM 작성 규칙

| 순서 |       속성       |                    의미                    | 관련 속성                                                                                      |
|:----:|:----------------:|:------------------------------------------:|------------------------------------------------------------------------------------------------|
|   1  |      display     |                    표시                    |                                           visibility                                           |
|   2  |     overflow     |                    넘침                    |                                                -                                               |
|   3  |       float      |                    흐름                    |                                              clear                                             |
|   4  |     position     |                    위치                    |                                                -                                               |
|   5  |      z-index     |                    정렬                    |                                top, right, left, bottom, z-index                               |
|   6  |  width & height  |                    크기                    |                                                -                                               |
|   7  | margin & padding |                    간격                    |                                                -                                               |
|   8  |      border      |                    보더                    |                                                                                                |
|   9  |       font       |                    폰트                    |                                                                                                |
|  10  |    background    |                    배경                    |                                                                                                |
|  11  |     etc(기타)    | color,text-decoration,text-indent,clear... | color, letter-spacing, text-align, text-decoration, text-indent, vertical-align, white-space등 |
---

1. font 속성 순서
    * 축약형을 사용하지 않으며, 스타일 선언시 font-style > font-variant > font-weight > font-size > line-height > font-family 순서로 선언하길 권장한다.

2. background-position 속성값
    * 숫자로 선언한다. ex).bg {background-position:100% 50%} (o)

3. 컬러값
    * 축약형을 사용한다. ex) .txt {color:#666} (o)

4. 공통 스타일시트
    * 크로스브라우징을 위해 각 태그관련 속성을 초기화 시켜주는 CSS로 PC와 Mobile에서의 환경을 고려하여 각각 reset.css를 정의하고 있다. 각 서비스 개편시 해당 reset.css를 활용하여 초기화시켜준다. 
