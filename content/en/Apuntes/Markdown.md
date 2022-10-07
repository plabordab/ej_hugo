---
title: "Markdown"
date: 2022-09-23T16:59:13+02:00
draft: false
---

# h1 Title 1
## h2 Title 2
### h3 Title 3
#### h4 Title 4
##### h5 Title 5
###### h6 Title 6

<!--
comment
-->

Any of the text that does not begin with a special sign will be written as normal, unformatted text, and will be wrapped inside <p></p> tags in the rendered HTML.

**bold**

_italic_

*italic*

***** bold and italic *****

~~strikethrough~~

~~***Strikethrough, Bold and Italics***~~

> To include quotes 
>
>> You can include quotations within quotations
> 
> And continue in the previous one

*Footnotes*

This year we will visit the Giralda[^1]. It will be an important visit.

*Definition of abbreviations:* 

TAS approved your application.

*[TAS]: Court of Arbitration for Sport.

From now on whenever we write TAS we will have its definition available.

*Word definition:*

Markdown
: It is a lightweight markup language created by John Gruber
: It is an English word meaning markdown.

#### **lists**


* enumeration 1
    - enumeration 2
        + enumeration 3

1. Lists
4. where
2. the
12. order
8. not
99. is
21. important

..

1. If you only use 1. 
1. for each number, 
1. Markdown will automatically number 
1. each element

#### **Code**

To highlight code within a sentence: `sudo apt install libreoffice`.

To include indentation we put at least two spaces:
    line 1 of code
    line 2 of code
    line 3 of code

``` 
We use quotation marks to write 
several lines of code
```

To highlight the syntax, we add the file extension of the language we want to use after the quotation marks.

```js
grunt.initConfig({
  assemble: {
    options: {
      assets: 'docs/assets',
      data: 'src/data/*.{json,yml}',
      helpers: 'src/custom-helpers.js',
      partials: ['src/partials/**/*.{hbs,md}']
    },
    pages: {
      options: {
        layout: 'default.hbs'
      },
      files: {
        './': ['src/templates/pages/index.hbs']
      }
    }
  }
};
```

#### **Tables**

| Time | Monday | Tuesday | Wednesday | Thursday | Friday|
| ------: | ------ | ------ | ------ | ------ | ------ | 
| 1 | Client | Deployment | ------ | Client | Server | 
| 2 | Client | Deployment | ------ | Client | Server | 
| 3 | Client | Server | Interfaces | Client | Server | 
| 4 | Interfaces | Server | Interfaces | Server | Interfaces | 
| 5 | Deployment | Server | ------ | Server | Interfaces | 
| 6 | Deployment | ------ | ------ | Server | Interfaces | 

The text is right-justified by placing : to the right of the dashes in the corresponding column.

**Task list 14-12-2019**

- [X] take the children swimming
- [X] learn markdown
- [ ] renew my gym membership


#### **Hyperlinks**

[Markdown syntax](https://geekland.eu/aprender-markdown-en-minutos/ "You can add a balloon with help info.")


**Tables of contents with anchors to the document**

- [Lists](#Lists)
- [Code](#Code)
- [Tables](#Tables)
- [Hyperlinks](#Hyperlinks)


![Image not found](/imagen/img1.jpeg "optional titl")

Between two text sections we can include a physical separation. To do this we have to write 3 underscores in a row 

___

> It is important to enter the alt value (alternative text if the image does not load) in the images.
>
> Create in the static folder the image folder
>
> In the public folder we save the whole structure from the static folder





[^1]: Name given to the bell tower of the cathedral of Santa Maria de la Sede.