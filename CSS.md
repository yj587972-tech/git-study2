
# CSS 정리

## 1. CSS란?

CSS(Cascading Style Sheets)는 HTML로 작성한 웹페이지의 디자인을 꾸미는 언어이다.

글자 색상, 크기, 배경색, 여백, 정렬 등을 설정할 수 있다.

## 2. CSS 적용 방식

### ① Inline CSS
HTML 태그 안에 style 속성을 직접 작성하는 방식이다.

예시:
```html
<p style="color: blue;">안녕하세요</p>
```

### ② Internal CSS
HTML 문서의 head 태그 안에 style 태그를 사용하여 작성하는 방식이다.

예시:
```html
<style>
p {
    color: blue;
}
</style>
```

### ③ External CSS
별도의 CSS 파일을 만들어 HTML과 연결하는 방식이다.

예시:
```html
<link rel="stylesheet" href="style.css">
```

여러 페이지에서 재사용하기 좋고 유지보수가 편리하다.

## 3. CSS Selector (선택자)

선택자는 HTML 요소 중 디자인을 적용할 대상을 선택하는 방법이다.

- 전체 선택자(*): 모든 요소 선택
- 태그 선택자: 특정 태그 선택 (예: p, h1)
- 클래스 선택자(.): 특정 클래스 선택
- 아이디 선택자(#): 특정 아이디 선택

예시:
```css
p {
    color: blue;
}

.title {
    font-size: 24px;
}

#header {
    background-color: lightgray;
}
```

## 4. Style 속성

### ① Text 관련 속성

- font-size: 글자 크기
- font-weight: 글자 굵기
- text-align: 글자 정렬

예시:
```css
p {
    font-size: 16px;
    font-weight: bold;
    text-align: center;
}
```

### ② Box Model

HTML 요소는 다음과 같은 구조로 이루어진다.

- Content: 실제 내용 영역
- Padding: 내용과 테두리 사이의 여백
- Border: 테두리
- Margin: 요소 바깥쪽 여백

주요 속성:

- width: 너비
- height: 높이
- margin: 바깥 여백
- padding: 안쪽 여백
- border: 테두리
- box-sizing: 요소 크기 계산 방식

예시:
```css
div {
    width: 300px;
    padding: 20px;
    border: 1px solid black;
    margin: 10px;
    box-sizing: border-box;
}
```

## 마무리

CSS를 사용하면 HTML 문서의 디자인을 다양하게 변경할 수 있다.

External CSS 방식을 사용하면 HTML과 디자인을 분리하여 관리할 수 있다.
