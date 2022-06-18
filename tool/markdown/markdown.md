# 마크다운

마크다운이란 메모를 작성하고 웹사이트용 컨텐츠를 작성하는데 유용한 마크업언어이다. <br>
블로그를 다시 시작하면서, 문서의 통일감을 맞추기 위해 먼저 작성한다.
<br>

## 1. 마크다운 문법
마크다운의 문법을 소개하는 글은 많지만,
차후에 참고하는 용도로 작성하는 글이기 때문에 <br>
[마크다운가이드](https://www.markdownguide.org/basic-syntax/)를 참고하여 작성한다.

### 1.1 Header
header는 제목을 표현할 때 사용하며, 크기에 따라 h1부터 h6까지 지원된다.

```html
# Headig level 1
## Headig level 2

또는

<h1>Headig level 1</h1>
<h2>Headig level 2</h2>

또는

Heading level 1
===============
Heading level 2
---------------
```


Heading level 1
===============
Heading level 2
---------------
<br>

### 1.2 Line Breaks
줄바꿈을 위해 \<br>을 사용한다.
```
<p>This is the first line.<br>
And this is the second line.</p>
```

<p>This is the first line.<br>
And this is the second line.</p>


### 1.3 Blockquotes
인용구는 >를 이용하여 표현한다.
~~~
> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
~~~
> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### 1.4 Lists
정렬, 비정렬로 구분되지만 동시에 사용가능하며, 굉장히 편리하다.
#### 1.4.1 Ordered Lists
~~~
1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item

또는

<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item
    <ol>
      <li>Indented item</li>
      <li>Indented item</li>
    </ol>
  </li>
  <li>Fourth item</li>
</ol>
~~~
1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item
#### 1.4.2 Unordered Lists
\-, *, +가 같은 용도로 사용된다.
~~~
- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item

또는

<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item
    <ul>
      <li>Indented item</li>
      <li>Indented item</li>
    </ul>
  </li>
  <li>Fourth item</li>
</ul>
~~~

- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item

### 1.5 Code Blocks
마크다운 문법을 벗어나서 작성할 수 있다.
```
1. Open the file.
2. Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3. Update the title to match the name of your website.

markdownguide.org에서는 위처럼 스페이스바 4번 또는 탭 1번으로 사용할 수 있다고 하지만,
```

~~~
```
이런식으로
```
~~~

```
~~~
사용하는것이 
~~~
```
편하다.

이때, 언어를 지정해 줄 수 있다.
~~~
```python
print('hello world')
```
~~~
```python
print('hello world')
```

### 1.6 Code & Escaping Backticks

```
At the command prompt, type `nano`.
또는
At the command prompt, type <code>nano</code>.

```
At the command prompt, type `nano`.

```
``Use `code` in your Markdown file.``
또는
<code>Use `code` in your Markdown file.</code>
```

``Use `code` in your Markdown file.``


+ 마크다운 문법 그대로 표현하기 위해 \를 이용한다.
  ~~~
  \### 예를들어
  ~~~
  \### 예를들어


### 1.7 Horizontal Rules
```
***

---

_________________
```
***

### 1.8 Links
```
My favorite search engine is [Google](https://www.google.com).
```
My favorite search engine is [Google](https://www.google.com).

링크를 빠르게 변환하거나, 강조할 때는 
```
<https://www.google.com>

I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).
```
<https://www.google.com>
<br>
I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).

### 1.9 Images
절대경로와 상대경로를 사용할 수 있다.
```
![이미지 불러오기 실패시 표기될 메세지](이미지주소)
```
```
![The San Juan Mountains are beautiful!](/assets/images/san-juan-mountains.jpg "San Juan Mountains")
```
![The San Juan Mountains are beautiful!](/assets/images/san-juan-mountains.jpg "San Juan Mountains")
<br>
이는 상대경로라서 표기되지 않는 모습.

```
![image](https://live.staticflickr.com/389/31833779864_373eecb0be_4k.jpg)
```
![image](https://live.staticflickr.com/389/31833779864_373eecb0be_4k.jpg)


### 1.10 Table
;를 이용하여 정렬을 조절 할 수 있다.
~~~
|기본값|왼쪽 정렬|가운데 정렬|오른쪽 정렬|
|---|:---|:---:|---:|
|내용 1|내용 2|내용 3|내용 4|
|내용 5|내용 6|내용 7|내용 8|
|내용 9|내용 10|내용 11|내용 12|
~~~
|기본값|왼쪽 정렬|가운데 정렬|오른쪽 정렬|
|---|:---|:---:|---:|
|내용 1|내용 2|내용 3|내용 4|
|내용 5|내용 6|내용 7|내용 8|
|내용 9|내용 10|내용 11|내용 12|

- 많이 사용하는 표 만들기 사이트 [tablesgenerator](https://www.tablesgenerator.com/markdown_tables)


***
## 2. vscode 확장
기존에 사용하던 typora에서 vscode로 마크다운을 사용하기 시작하면서 설치함.
### 2.1 markdownlint
 - 마크다운으로 다양한 양식으로 작성 가능하기 때문에, 표준 및 일관성을 위해 사용.
  https://github.com/DavidAnson/vscode-markdownlint)

### 2.2 Markdown All in one
  - vscode에서 markdown을 지원을 기본적으로 제공하지만, 단축키, 목차, 자동미리보기 등을 제공 
  https://github.com/yzhang-gh/vscode-markdown
