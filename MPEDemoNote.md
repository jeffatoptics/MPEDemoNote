---
chrome:
    printBackground: true
    format: "A4"
html:
    toc: true
---

<!--- 
chrome.format: use "A3" for wider print, or use  "tabloid"
--->


# MPE Demo Note {ignore}

[TOC]

## Reference Link

- [markdown guide](https://www.markdownguide.org/getting-started/)
- [markdown preview enhanced](https://shd101wyy.github.io/markdown-preview-enhanced/#/)
- [markdown cheat sheet](https://www.markdownguide.org/cheat-sheet/)
- [markdown cheat sheet md file](https://www.markdownguide.org/assets/markdown-cheat-sheet.md)


## Front settings 

- chrome print settings

```
---
chrome:
    printBackground: true
    format: "A4"
---

```
- html output settings

```
---
html:
    embed_local_images: false
    embed_svg: true
    offline: false
    toc: true
    print_background: false
---

```

- PanDoc Print Settings

```
---
title: "this_is_title"
author: author_name
date: Jan 14, 2022
output:	
    word_document:
        highlight: "tango"
---

```

## Definition  

GitHub
    : GitHub is a website with Git tool

## Abbreviation 
*[YYDS]: Yong Yuan De Shen - God forever
YYDS

## footnote

Demo[^1] a footnote

[^1]: this a footnote

## comment

1. html comment
    <!---
    this is my comment 
    -->
    ```
    <!---
    your comment goes here
    and here
    -->
    ```
1. markdown
    ```
    (empty line)
    [comment]: # (This actually is the most platform independent comment)
    ```
    [comment]: # (this is a comment)

1. markdown

    [this is comment]: #

    ```
    [this is a comment]: #
    ```


1. footnote no referenced
    ```
    [^Comment]:  Text that will not appear in html source
    ```
    [^Comment]:  Text that will not appear in html source
    
## emoji and html symbol
- Reference link: [html symbol](https://www.toptal.com/designers/htmlarrows/)

- `&micro;` time is 10&micro;s 
- `&deg;` temperature is 20&deg;
- `&plusmn;`&plusmn;25
- `&le; &ge; &ne;` &le; &ge; &ne;
- `&trade; &reg;`  Google&trade; &reg;Google
- `&copy;` &copy;2002
- `&raquo;&laquo;` &raquo; &laquo;
- `&nbsp;&nbsp;&nbsp;&nbsp;` &nbsp;&nbsp;&nbsp;&nbsp;

- positive signs: 
    - :+1: :100: :joy: :accept: :heart: :beer: :beers: :white_check_mark:
    - `:+1: :100: :joy: :accept: :heart: :beer: :beers: :white_check_mark:`
    - :ok: `:ok:`
    
- neutral
    - :eyes: :alien: :confused:
    - `:eyes: :alien: :confused:`
- negative
    - :-1: :angry: :sweat: :sob: `:-1: :angry: :sweat: :sob: `
    - :broken_heart: `:broken_heart:`
    - :bug: `:bug:`
- Informational
    - :memo:`:memo`
    - :question: `:question:`
    - :no_entry: :no_entry_sign:  `:no_entry: :no_entry_sign:`
    - :bookmark_tabs: :information_source: :warning: `:bookmark_tabs: :information_source: :warning:`
    - :arrow_right: :arrow_left: :arrow_up: :arrow_down: `:arrow_right: :arrow_left: :arrow_up: :arrow_down`
    - :ballot_box_with_check:`:ballot_box_with_check:`
    - &rarr; &larr; &uarr; &darr; `&rarr; &larr; &uarr; &darr;`
    - :bangbang: `:bangbang: `
    - :boom: `:boom:`
    - :chart_with_downwards_trend: :chart_with_upwards_trend: `:chart_with_downwards_trend: :chart_with_upwards_trend:`
    - :page_with_curl: `:page_with_curl:`
    - :link: `:link:`
    - ❌ `:x:`

## List Level Demo {#section11}

- This is a list level 1
    - this is a list level 2
    - this is a list level 2
        - this a list level 3
- This is a list level 1

1. This is a list level 1
    - this is a list level 2
        - this is a list level 3
1. this is a list level 1
    - this is a list level 2

## Horizontal Line Demo

---

this is a demo

---

```
(empty line)
---
(empty line)
text
(empty line)
---
(empty line)
```

***
this is a demo
***

```

***

text

***

```

## link demo

- [demo the link within the doc](#horizontal-line-demo)

```
[demo the link within the doc](#horizontal-line-demo)
```
- [demo the link within the doc use the id](#section11)

```
[demo the link within the doc use the id](#id)
id is using the #xxx{id}

### My Great Heading {#custom-id}
```

- [demo the link to another file](./README.md)

```
[demo the link to another file](./README.md)
```
- [demo the link to another file](./README.md#mpedemonote)

```
- [demo the link to section in another file](./README.md#mpedemonote)

```
- [demo the external link](https://github.com/jeffatoptics/MPEDemoNote)

- <https://github.com/jeffatoptics/MPEDemoNote>

## html syntax

- <mark> this is a mark</mark>
- ==this is a mark==

- <b>this is bold</b>
- **bold**

- <u> this is underline</u>
- <ins>will be underlined</ins>

- <i>this is italic</i>
- _this is italic_

- <s>test</s>
- ~~test~~

- <font color=red>test</font>
- <p style="color:blue">Make this text blue.</p>

- H<sub>2</sub>O
- H~2~O

- Y=X^2^

- Y=X<sup>2</sup>

- [x] task list

- [ ] task list 

## definition

term
: this is for a demo of definition






## Code Demo 

- language: python, cmd, bash, diff, c, json

``` {.line-numbers, highlight=[2,3,6-7]}
import numpy, math
a="this is a text"
print (a)
b=math.pi
c=a+a
for i in a
    print(i)

```

```diff {.line-numbers}
# this is a demo text
config interface 1/1/line state donw
+ print ("this is done")
- print ("this is not done") 

```


## Admonitions

```
> :warning: **Warning:** Do not push the big red button.

> :memo: **Note:** Sunrises are beautiful.

> :bulb: **Tip:** Remember to appreciate the little things in life.
```
> :warning: **Warning:** Do not push the big red button.

> :memo: **Note:** Sunrises are beautiful.

> :bulb: **Tip:** Remember to appreciate the little things in life.

> :question: This is a question

> :heavy_check_mark: success

> :white_check_mark: success

> :x: this is a failure

!!!warning this is a warning
    text to put

!!!note this is a note
    text to put

!!!info this is an info
    text to put    

!!!abstract this is an abstract
    text to put    

!!!tip this is an info
    text to put  

!!! Success

!!! Question

!!! Failure

!!! Danger

!!! Bug

!!! Example
    
!!! Quote

```

 Note
 Abstract
 Inf
 Tip
 Success
 Question
 Warning
 Failure
 Danger
 Bug
 Example
 Quote

```  


## Math 

- [Math symbols](https://khan.github.io/KaTeX/function-support.html)

- This is an inline equation: $ y=\sqrt{x^2-1} $ and $ y=\sqrt[4]{x^2-1} $
- This is an equation block
    $$
    y=\frac{1}{2} \times \sqrt{x^2-1} \\
    y=\cfrac{1}{2+\cfrac{1}{2}}     \\
    y=\int \! (x^2-1) dx             \\
    y=\int (x^2-1) dx                \\
    y=\int_{a}^{b=10} (x^2-1) dx            \\
    y=\sum_{x=1}^ {100} (x^2-1)- 1          \\
    BER= erfc(\frac{Q}{\sqrt(2)})
    $$
 
$$
\fbox {this is a demo equation: }   \\
BER= erfc(\frac{Q}{\sqrt(2)})
$$


## mermaid

```mermaid
graph LR
A(This is A)----->|this is demo text|B[(this is database<br><br> demo)]
C((This is C))--this is demo text--->B
D{This is D}--this is demo text--->B

    subgraph box
        A---C----D
        subgraph newbox
        C
        D
        end
    end
    subgraph box2
    B
    end
style B fill:#bbf,stroke:#000,stroke-width:4px,color:#f00,stroke-dasharray: 10 2
linkStyle 0 stroke:#f00,stroke-width:4px
```

```mermaid
flowchart LR
A<==>B<-..->C
A[this is a text]
B[this is demo]
style B fill:#bbf

```

```mermaid
pie
    title Bugs in Software
    "transmission" : 15.00
    "alarm" : 25
    "management" : 66
    "performance" : 5
```


```mermaid
gantt
    title A Gantt Diagram
    dateFormat  YY-MM-DD
    axisFormat   %y-%m-%d
    section Section 1
    A task           :done, a1, 21-12-01, 20d
    Another task     :active, after a1, 60d
    section Section 2
    B      :crit,22-02-12, 20d
    milestone: milestone,20d
```

```mermaid
gantt
    title A Gantt Diagram
    dateFormat  YY-MM-DD
    axisFormat   %y-%m-%d
    section Section 1
    A task           :done, a1, 21-12-01, 20d
    Another task     :active, after a1, 60d
    section Section 2
    B      :crit,22-02-12, 20d
    milestone: milestone,20d
```
