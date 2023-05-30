---
title: 복잡한 문자열 합치기
description: "C# 복잡한 문자열 합치기를 보기쉽게"
---

보통 문자열을 합칠 때 쓰는 방법이 있다 

```cs
int winner = 10; 
string str = "승자는 : " + winner + "번 선수 입니다.";
```

하지만 이 문자열은 가독성이 떨어지고, +를 넣어야 되는 노가다를 많이 할 수 있다.

그래서 대신 아래와 같은 문자열을 사용 할 수 있다

```cs
int winner = 10;
string str = $"승자는 : {winner}번 선수 입니다.";
```

[//]: # (![png]&#40;./code.png&#41;)

[//]: # (You can also write code blocks here!)

[//]: # ()
[//]: # (```js)

[//]: # (const saltyDuckEgg = "chinese preserved food product")

[//]: # (```)

[//]: # ()
[//]: # (| Number | Title                                    | Year |)

[//]: # (| :----- | :--------------------------------------- | ---: |)

[//]: # (| 1      | Harry Potter and the Philosopher’s Stone | 2001 |)

[//]: # (| 2      | Harry Potter and the Chamber of Secrets  | 2002 |)

[//]: # (| 3      | Harry Potter and the Prisoner of Azkaban | 2004 |)

[//]: # ()
[//]: # ([View raw &#40;TEST.md&#41;]&#40;https://raw.github.com/adamschwartz/github-markdown-kitchen-sink/master/README.md&#41;)

[//]: # ()
[//]: # (This is a paragraph.)

[//]: # ()
[//]: # (    This is a paragraph.)

[//]: # ()
[//]: # (# Header 1)

[//]: # ()
[//]: # (## Header 2)

[//]: # ()
[//]: # (    Header 1)

[//]: # (    ========)

[//]: # ()
[//]: # (    Header 2)

[//]: # (    --------)

[//]: # ()
[//]: # (# Header 1)

[//]: # ()
[//]: # (## Header 2)

[//]: # ()
[//]: # (### Header 3)

[//]: # ()
[//]: # (#### Header 4)

[//]: # ()
[//]: # (##### Header 5)

[//]: # ()
[//]: # (###### Header 6)

[//]: # ()
[//]: # (    # Header 1)

[//]: # (    ## Header 2)

[//]: # (    ### Header 3)

[//]: # (    #### Header 4)

[//]: # (    ##### Header 5)

[//]: # (    ###### Header 6)

[//]: # ()
[//]: # (# Header 1)

[//]: # ()
[//]: # (## Header 2)

[//]: # ()
[//]: # (### Header 3)

[//]: # ()
[//]: # (#### Header 4)

[//]: # ()
[//]: # (##### Header 5)

[//]: # ()
[//]: # (###### Header 6)

[//]: # ()
[//]: # (    # Header 1 #)

[//]: # (    ## Header 2 ##)

[//]: # (    ### Header 3 ###)

[//]: # (    #### Header 4 ####)

[//]: # (    ##### Header 5 #####)

[//]: # (    ###### Header 6 ######)

[//]: # ()
[//]: # (> Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.)

[//]: # ()
[//]: # (    > Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.)

[//]: # ()
[//]: # (> ## This is a header.)

[//]: # (>)

[//]: # (> 1. This is the first list item.)

[//]: # (> 2. This is the second list item.)

[//]: # (>)

[//]: # (> Here's some example code:)

[//]: # (>)

[//]: # (>     Markdown.generate&#40;&#41;;)

[//]: # ()
[//]: # (    > ## This is a header.)

[//]: # (    > 1. This is the first list item.)

[//]: # (    > 2. This is the second list item.)

[//]: # (    >)

[//]: # (    > Here's some example code:)

[//]: # (    >)

[//]: # (    >     Markdown.generate&#40;&#41;;)

[//]: # ()
[//]: # (- Red)

[//]: # (- Green)

[//]: # (- Blue)

[//]: # ()
[//]: # (* Red)

[//]: # (* Green)

[//]: # (* Blue)

[//]: # ()
[//]: # (- Red)

[//]: # (- Green)

[//]: # (- Blue)

[//]: # ()
[//]: # (```markdown)

[//]: # (- Red)

[//]: # (- Green)

[//]: # (- Blue)

[//]: # ()
[//]: # (* Red)

[//]: # (* Green)

[//]: # (* Blue)

[//]: # ()
[//]: # (- Red)

[//]: # (- Green)

[//]: # (- Blue)

[//]: # (```)

[//]: # ()
[//]: # (- `code goes` here in this line)

[//]: # (- **bold** goes here)

[//]: # ()
[//]: # (```markdown)

[//]: # (- `code goes` here in this line)

[//]: # (- **bold** goes here)

[//]: # (```)

[//]: # ()
[//]: # (1. Buy flour and salt)

[//]: # (1. Mix together with water)

[//]: # (1. Bake)

[//]: # ()
[//]: # (```markdown)

[//]: # (1. Buy flour and salt)

[//]: # (1. Mix together with water)

[//]: # (1. Bake)

[//]: # (```)

[//]: # ()
[//]: # (1. `code goes` here in this line)

[//]: # (1. **bold** goes here)

[//]: # ()
[//]: # (```markdown)

[//]: # (1. `code goes` here in this line)

[//]: # (1. **bold** goes here)

[//]: # (```)

[//]: # ()
[//]: # (Paragraph:)

[//]: # ()
[//]: # (    Code)

[//]: # ()
[//]: # (<!-- -->)

[//]: # ()
[//]: # (    Paragraph:)

[//]: # ()
[//]: # (        Code)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (    * * *)

[//]: # ()
[//]: # (    ***)

[//]: # ()
[//]: # (    *****)

[//]: # ()
[//]: # (    - - -)

[//]: # ()
[//]: # (    ---------------------------------------)

[//]: # ()
[//]: # (This is [an example]&#40;http://example.com "Example"&#41; link.)

[//]: # ()
[//]: # ([This link]&#40;http://example.com&#41; has no title attr.)

[//]: # ()
[//]: # (This is [an example][id] reference-style link.)

[//]: # ()
[//]: # ([id]: http://example.com "Optional Title")

[//]: # ()
[//]: # (    This is [an example]&#40;http://example.com "Example"&#41; link.)

[//]: # ()
[//]: # (    [This link]&#40;http://example.com&#41; has no title attr.)

[//]: # ()
[//]: # (    This is [an example] [id] reference-style link.)

[//]: # ()
[//]: # (    [id]: http://example.com "Optional Title")

[//]: # ()
[//]: # (_single asterisks_)

[//]: # ()
[//]: # (_single underscores_)

[//]: # ()
[//]: # (**double asterisks**)

[//]: # ()
[//]: # (**double underscores**)

[//]: # ()
[//]: # (    *single asterisks*)

[//]: # ()
[//]: # (    _single underscores_)

[//]: # ()
[//]: # (    **double asterisks**)

[//]: # ()
[//]: # (    __double underscores__)

[//]: # ()
[//]: # (This paragraph has some `code` in it.)

[//]: # ()
[//]: # (    This paragraph has some `code` in it.)

[//]: # ()
[//]: # (![Alt Text]&#40;https://via.placeholder.com/200x50 "Image Title"&#41;)

[//]: # ()
[//]: # (    ![Alt Text]&#40;https://via.placeholder.com/200x50 "Image Title"&#41;)
