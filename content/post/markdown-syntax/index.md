+++
author = "Wontory"
title = "마크다운 문법 정리 (Markdown Syntax)"
date = "2022-08-01"
description = "마크다운, 서식이 있는 문서를 작성하는 쉽고 편리한 언어"
tags = [
    "markdown",
    "syntax", 
    "themes",
]
categories = [
    "language",
]
slug = "markdown-syntax"
series = [
  "Themes Guide"
]
image = "markdown_banner.png"
+++

본 문서는 Hugo 및 Github Pages 포스팅을 위한 마크다운 문법을 서술합니다.
<!--more-->

&nbsp;

## 제목(Headings)

HTML `<h1>`---`<h6>` 요소는 6가지 수준의 섹션 제목을 나타냅니다. `<h1>`부터 `<h6>`까지 순서대로 높은 섹션 수준을 갖습니다. 마크다운에서는 제목 앞 `#` 기호의 개수로 섹션 수준을 구분합니다.

#### 제목 예시
TOC 문제로 이미지로 대체합니다. (실제 크기와 다를 수 있습니다.)  

![](headings_sample.png)

**\[ Code \]**

```markdown
# 제목1
## 제목2
### 제목3
#### 제목4
##### 제목5
###### 제목6
```

&nbsp;

## 문단(Paragraphs)

문단을 구분할 때는 두 문단 사이에 **빈 줄**을 추가합니다.

#### 문단 예시

계절이 지나가는 하늘에는 가을로 가득 차 있습니다.  
나는 아무 걱정도 없이 가을 속의 별들을 다 헤일 듯합니다.  
가슴 속에 하나 둘 새겨지는 별을 이제 다 못 헤는 것은  
쉬이 아침이 오는 까닭이요, 내일 밤이 남은 까닭이요,  
아직 나의 청춘이 다하지 않은 까닭입니다.  

별 하나에 추억과 별 하나에 사랑과  
별 하나에 쓸쓸함과 별 하나에 동경과  
별 하나에 시와 별 하나에 어머니, 어머니

**\[ Code \]**

```markdown
계절이 지나가는 하늘에는 가을로 가득 차 있습니다.  
나는 아무 걱정도 없이 가을 속의 별들을 다 헤일 듯합니다.  
가슴 속에 하나 둘 새겨지는 별을 이제 다 못 헤는 것은  
쉬이 아침이 오는 까닭이요, 내일 밤이 남은 까닭이요,  
아직 나의 청춘이 다하지 않은 까닭입니다.  

별 하나에 추억과 별 하나에 사랑과  
별 하나에 쓸쓸함과 별 하나에 동경과  
별 하나에 시와 별 하나에 어머니, 어머니
```

&nbsp;

## 줄 바꿈(Line Breaks)

문장 끝에 스페이스 바로 **2개 이상 공백**을 넣어 줄 바꿈을 할 수 있습니다.

#### 줄 바꿈 예시

"그만 거둘까?"  
"잘 생각했네.봉평장에서 한번이나 흐뭇하게 사본 일 있을까.내일 대화장에서나 한몫 벌어야겠네."  
"오늘밤은 밤을 새서 걸어야 될걸?"  
"달이 뜨렷다?"

**\[ Code \]**

```markdown
"그만 거둘까?"  
"잘 생각했네.봉평장에서 한번이나 흐뭇하게 사본 일 있을까.내일 대화장에서나 한몫 벌어야겠네."  
"오늘밤은 밤을 새서 걸어야 될걸?"  
"달이 뜨렷다?"
```

&nbsp;

## 구분선(Horizontal Rules)

`*` 기호, `-` 기호, `_` 기호를 **3개 이상** 작성하여 구분선을 표시할 수 있습니다.

#### 구분선 예시

***

---

_____________

**\[ Code \]**

```markdown
***

---

_____________
```

&nbsp;

## 인용문(Blockquotes)

`<blockquote>` 요소는 안쪽의 텍스트가 긴 인용문임을 나타내며, 일반적으로 들여쓰기가 적용됩니다. `<footer>`나 `<cite>` 요소를 인용문에 선택적으로 적용할 수 있고, **주석**이나 **약어**를 포함할 수 있습니다.

#### 인용문 예시

> **단순함**은 *복잡함*보다 더 어렵다.  
> 생각을 명확히 하고 단순하게 만들려면 열심히 노력해야 한다.  
> 생각을 단순하게 만들 수 있는 단계에 도달하면 산도 움직일 수 있다.  
> --- <cite>스티브 잡스[^1]</cite>

[^1]: 故 스티브 잡스, Business Week(1998)

**\[ Code \]**

```markdown
> **단순함**은 *복잡함*보다 더 어렵다. 
> 생각을 명확히 하고 단순하게 만들려면 열심히 노력해야 한다.  
> 생각을 단순하게 만들 수 있는 단계에 도달하면 산도 움직일 수 있다.
> --- <cite>스티브 잡스[^1]</cite>

[^1]: 故 스티브 잡스, Business Week(1998)
```

&nbsp;

## 표(Tables)

표는 마크다운에서 확장 기능으로 제공하고 있습니다. 인용문과 마찬가지로, 표 내에서 마크다운 문법을 사용할 수 있습니다. `|` 기호로 행을 구분하고 `-` 기호로 열을 구분합니다. 이 때, `-` 기호는 **3개 이상** 사용해야 합니다.

#### 표 예시

| 이름 | 나이 |
| --- | --- |
| Wontory | 23 |
| 네이버 | 24 |
| 카카오 | 13 |

**\[ Code \]**

```markdown
| 이름 | 나이 |
| --- | --- |
| Wontory | 23 |
| 네이버 | 24 |
| 카카오 | 13 |
```

#### 표 내 마크다운 예시

| Italic | Bold | Bold and Italic | Code |
| --- | --- | --- | --- |
| *italic* | **bold** | ***bold and italic*** | `code` |

**\[ Code \]**

```markdown
| Italic | Bold | Bold and Italic | Code |
| --- | --- | --- | --- |
| *italic* | **bold** | ***bold and italic*** | `code` |
```

&nbsp;

## 코드 블럭(Code Blocks)

일반적으로 코드는 **\` 기호 1개**로 묶어 사용하지만, 여러 줄의 코드를 블로그에 삽입할 때는 코드 블럭을 사용합니다. 코드 블럭은 **Syntax Highlight**를 지원하여 코드를 더 보기 쉽게 정리할 수 있습니다.

#### \` 기호(Backtick)를 사용한 코드 블럭 예시

코드를 **\` 기호 3개**로 감싸고 **언어를 지정**해주면 코드 블럭이 활성화됩니다. 언어를 지정하지 않아도 코드 블럭을 사용할 수 있지만, Syntax Highlight는 사용할 수 없습니다.

```html
<!doctype html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <title>HTML5 코드 예시</title>
</head>
<body>
  <p>예시</p>
</body>
</html>
```

**\[ Code \]**

{{< highlight markdown >}}
```html
<!doctype html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <title>HTML5 코드 예시</title>
</head>
<body>
  <p>예시</p>
</body>
</html>
```
{{< /highlight >}}

#### 들여쓰기를 이용한 코드 블럭 예시

**4칸 이상 들여쓰기**를 하여 코드 블럭을 적용할 수 있습니다. 강조와 줄 번호가 표시되지 않는 특징이 있습니다.

    <!doctype html>
    <html lang="ko">
    <head>
      <meta charset="utf-8">
      <title>HTML5 코드 예시</title>
    </head>
    <body>
      <p>예시</p>
    </body>
    </html>

**\[ Code \]**

{{< highlight markdown >}}
    <!doctype html>
    <html lang="ko">
    <head>
      <meta charset="utf-8">
      <title>HTML5 코드 예시</title>
    </head>
    <body>
      <p>예시</p>
    </body>
    </html>
{{< /highlight >}}

#### Chroma Syntax Highlighter를 이용한 코드 블럭 예시

다음은 외부 Syntax Highlighter를 블로그에 적용했을 경우에만 해당합니다. Chroma의 경우, 사용법은 다음과 같습니다.

{{< highlight html >}}
<!doctype html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <title>HTML5 코드 예시</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

**\[ Code \]**

```markdown
{{</* highlight html */>}}
<!doctype html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <title>HTML5 코드 예시</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{</* /highlight */>}}
```

#### Diff 코드 블럭 예시

마크다운은 Diff를 지원하여 **코드의 변경사항**을 표기할 수 있습니다.

```diff
int main()
{
- printf("Hi, I'm Wrongtory.");
+ printf("Hi, I'm Wontory.");
}
```

**\[ Code \]**

{{< highlight markdown >}}
```diff
int main()
{
- printf("Hi, I'm Wrongtory.");
+ printf("Hi, I'm Wontory.");
}
```
{{< /highlight >}}

&nbsp;

## 목록(Lists)

#### 순서가 있는 목록 예시

1. 첫 번째 항목
2. 두 번째 항목
3. 세 번째 항목

**\[ Code \]**

```markdown
1. 첫 번째 항목
2. 두 번째 항목
3. 세 번째 항목
```

#### 순서가 없는 목록 예시

* 항목
* 다른 항목
* 또 다른 항목

+ 항목
+ 다른 항목
+ 또 다른 항목

- 항목
- 다른 항목
- 또 다른 항목

**\[ Code \]**

```markdown
* 항목
* 다른 항목
* 또 다른 항목

+ 항목
+ 다른 항목
+ 또 다른 항목

- 항목
- 다른 항목
- 또 다른 항목
```

#### 중첩 목록 예시

들여쓰기를 통해 목록을 중첩 사용할 수 있습니다.

* 과일
  * 사과
  * 오렌지
  * 바나나
* 유제품
  1. 우유
  2. 치즈

**\[ Code \]**

```markdown
* 과일
  * 사과
  * 오렌지
  * 바나나
* 유제품
  1. 우유
  2. 치즈
```

&nbsp;

## 하이퍼링크 이미지(Linking Images)

이미지를 추가할 때는 `![이미지 설명](이미지 경로)`와 같이 입력하면 됩니다. 하이퍼링크 양식인 `[주소 설명](주소)` 앞에 ! 기호를 추가한 것과 같습니다. 이미지 양식을 하이퍼링크 양식 안으로 넣어주면 이미지에 하이퍼링크를 적용할 수 있습니다.

#### 하이퍼링크 이미지 예시

[![Google](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)](https://google.com)

**\[ Code \]**

```markdown
[![Google](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)](https://google.com)
```