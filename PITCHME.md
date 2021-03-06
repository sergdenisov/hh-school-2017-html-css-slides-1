#HSLIDE

### HTML/CSS, часть 1

![HTML5/CSS3](images/HTML-CSS3.jpg)

Сергей Денисов

Старший фронтенд-разработчик


06.02.2017

#HSLIDE

### HTML5

* Последняя версия языка гипертекстовой разметки —
[HyperText Markup Language (HTML)](https://developer.mozilla.org/en-US/docs/Web/HTML), который используется для создания
и визуального представления веб-страниц.

* [Набор технологий (APIs)](https://developer.mozilla.org/en-US/docs/Web), позволяющих создавать разнообразные сайты и
Web-приложения: [Audio](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API),
[Video](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content),
[Drag and Drop](https://developer.mozilla.org/en-US/docs/Web/API/HTML_Drag_and_Drop_API) и т.д.

#HSLIDE

### [WC3/WHATWG](http://edgeatx.github.io/slides/2015/03-mar/#slide-18)

![WC3/WHATWG](images/w3c-whatwg.jpg)

#VSLIDE

* [Консорциум Всемирной паутины (W3C)](https://ru.wikipedia.org/wiki/%D0%9A%D0%BE%D0%BD%D1%81%D0%BE%D1%80%D1%86%D0%B8%D1%83%D0%BC_%D0%92%D1%81%D0%B5%D0%BC%D0%B8%D1%80%D0%BD%D0%BE%D0%B9_%D0%BF%D0%B0%D1%83%D1%82%D0%B8%D0%BD%D1%8B)
(World Wide Web Consortium) — организация, разрабатывающая и внедряющая стандарты для
Всемирной паутины. Консорциум возглавляет сэр Тимоти Джон Бернерс-Ли.

* [WHATWG](https://ru.wikipedia.org/wiki/WHATWG) (Web Hypertext Application Technology Working Group) — сообщество
людей, заинтересованных в развитии Интернета. Оно было основано в 2004 году производителями
браузеров: Apple, Mozilla Foundation и Opera Software.

#HSLIDE

### HTML: [Doctype](https://developer.mozilla.org/en-US/docs/Glossary/doctype)

* HTML 4:

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN"
          "http://www.w3.org/TR/html4/strict.dtd">
```

* HTML 5:

```html
<!DOCTYPE html>
```

#HSLIDE

### HTML: [элементы](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started#Anatomy_of_an_HTML_element) и [атрибуты](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started#Attributes)

![HTML Element](images/anatomy-of-an-html-element.png)

#VSLIDE

Элемент может быть:

* Быть пустым:

```html
<input type="button"/>
```

* Содержать другие элементы:

```html
<ul>
    <li>Element 1</li>
    <li>Element 2</li>
    ...
</ul>
```

#VSLIDE

* [Валидные элементы](https://developer.mozilla.org/en-US/docs/Web/HTML/Element).

* [Валидные атрибуты](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes).

#HSLIDE

### HTML: [категории контента](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories)

![Content categories](images/Content_categories_venn.png)

+[Basic element (root)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element#Basic_elements): `<html>`

#VSLIDE

### [Flow content](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Flow_content)

```html
<div>, <header>, <main>, <footer>, <ol>, <p>, <table>, <ul>
```

[Пример](https://jsfiddle.net/sergdenisov/v82gyp69/):

```html
<div>Text</div>
<p>Paragraph with content</p>
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>
```

#VSLIDE

### [Phrasing content](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Phrasing_content)

```html
<b>, <em>, <i>, <span>, <strong>, <sub>, <sup>
```

[Пример](https://jsfiddle.net/sergdenisov/kLttvwat/):

```html
<b>Bold text</b>
<em>Emphasis text</em>
<span>Simple text</span>
```

#VSLIDE

### [Metadata content](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Metadata_content)

```html
<meta>, <script>, <style>, <title>
```

Пример:

```html
<meta charset="utf-8"/>
<title>Awesome page title</title>
<script src="javascript.js"></script>
```

#VSLIDE

### [Sectioning content](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Sectioning_content)

```html
<article>, <aside>, <nav>, <section>
```

[Пример](https://jsfiddle.net/sergdenisov/mk1ttLd6/1/):

```html
<article>
    <p>
        The Disney movie <em>The Little Mermaid</em> was
        first released to theatres in 1989.
    </p>
    <aside>
        <p>
            The movie earned $87 million during its initial
            release.
        </p>
    </aside>
    <p>More info about the movie...</p>
</article>
```

#VSLIDE

### [Heading content](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Heading_content)

```html
<h1>, <h2>, <h3>, <h4>, <h5>, <h6>
```

[Пример](https://jsfiddle.net/sergdenisov/eymartn0/):

```html
<h1>Main title</h1>
<h2>Second title</h2>
<h3>Third title</h3>
<h4>Fourth title</h4>
<h5>Fifth title</h5>
<h6>Sixth title</h6>
```

#VSLIDE

### [Embedded content](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Embedded_content)

```html
<audio>, <canvas>, <iframe>, <img>, <svg>, <video>
```

[Пример](https://jsfiddle.net/sergdenisov/da5yxs2u/):

```html
<img src="https://jsfiddle.net/img/logo@2x.png"/>
<iframe width="560" height="315"
        src="https://www.youtube.com/embed/wn1Cvo43ri8"
        frameborder="0" allowfullscreen>
</iframe>
```

#VSLIDE

### [Interactive content](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Interactive_content)

```html
<a>, <button>, <label>, <select>, <textarea>
```

[Пример](https://jsfiddle.net/sergdenisov/40pdozdb/):

```html
<a href="https://hh.ru">HeadHunter link</a>
<label>
    Choose:
    <select>
        <option value="1">One</option>
        <option value="2">Two</option>
    </select>
</label>
```

#VSLIDE

### [Form-associated content](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Form-associated_content)

```html
<button>, <fieldset>, <input>, <label>, <select>, <textarea>
```

Пример:

```html
<form action="https://hh.ru/search/vacancy" method="get">
    <label>Vacancy name:
        <input type="text" name="text"/>
    </label>
    <input type="hidden" name="area" value="1"/>
    <button type="submit">Search</button>
</form>
```

#HSLIDE

### HTML: [типы атрибутов](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes)

* [Глобальные](https://developer.mozilla.org/en/docs/Web/HTML/Global_attributes) — применимы к любому элементу.

```
id, class, contenteditable, data-*
```

* [Обязательные для определенного элемента](https://developer.mozilla.org/en/docs/Web/HTML/Element/a#attr-href).

```html
<a href="https://www.google.ru">Search</a> 
```

* [Опциональные для определенного элемента](https://developer.mozilla.org/en/docs/Web/HTML/Element/button#attr-type).

```html
<button type="button">Click me</button>
```

#HSLIDE

### HTML: [комментарии](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started#HTML_comments) и [специальные символы (entities)](https://developer.mozilla.org/en-US/docs/Glossary/Entity)

```html
&nbsp; <!-- неразрывный пробел -->
 &quot; <!-- " --> 
&lt; <!-- < -->
 &gt; <!-- > —>
```

[Пример](https://jsfiddle.net/sergdenisov/rtvj546h/):

```html
<div>Фамилия&nbsp;Имя&nbsp;Отчество</div> <!-- Неразрывный -->
<div>Фамилия Имя Отчество</div> <!-- Обычный -->
```

#HSLIDE

### HTML: минимальный [валидный документ](https://validator.w3.org/#validate_by_input)

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Hello, World!</title>
    </head>
    <body>Hello, World!</body>
</html>
```

#HSLIDE

### HTML: [рекомендации](https://google.github.io/styleguide/htmlcssguide.xml#HTML_Style_Rules)

* Соблюдайте [валидность](https://google.github.io/styleguide/htmlcssguide.xml?showone=HTML_Validity#HTML_Validity)
документа.
* Верстайте [семантично](https://google.github.io/styleguide/htmlcssguide.xml?showone=Semantics#Semantics).
* Пишите весь код в [нижнем регистре](https://google.github.io/styleguide/htmlcssguide.xml?showone=Capitalization#Capitalization).
* Используйте [двойные кавычки](https://google.github.io/styleguide/htmlcssguide.xml?showone=HTML_Quotation_Marks#HTML_Quotation_Marks).
* Ознакомьтесь с [Google HTML Style Guide](https://google.github.io/styleguide/htmlcssguide.xml#HTML_Style_Rules).

#HSLIDE

### [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)

[CSS](https://developer.mozilla.org/en-US/docs/Web/CSS) (Cascading Style Sheets — каскадные таблицы стилей) — формальный
язык описания внешнего вида документа, написанного с использованием языка разметки.

![CSS3](images/css3.png)
![W3C](images/w3c.jpg)

#VSLIDE

Профит:

* Разделение контента и представления.
* Уменьшение дублирования кода.
* Упрощение поддержку.
* Уменьшение трафика.

#HSLIDE

### CSS: подключение

* Атрибут [style](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/style):

```html
<div style="color: red">Red text</div>
```

* Элемент [style](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/style):

```html
<style>
    body { 
        color: red;
    }
</style>
```

* Отдельным файлом через элемент [link](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link):

```html
<link href="style.css" rel="stylesheet"/>
```

#HSLIDE

### [Упрощенная схема работы браузера](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/How_CSS_works#How_does_CSS_actually_work)

![Rendering](images/rendering.png)

Подробнее: [презентация](http://arvindr21.github.io/howBrowserWorks/#/),
[статья](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/).

#HSLIDE

### CSS: [синтаксис](https://developer.mozilla.org/en-US/docs/Web/CSS/Syntax)

![CSS Syntax: Declaration](images/css-syntax-declaration.png)

#VSLIDE

![CSS Syntax: Declarations block](images/css-syntax-declarations-block.png)

#HSLIDE

### CSS: [типы значений](https://developer.mozilla.org/en/docs/Web/CSS/Value_definition_syntax)

* [Ключевые слова](https://developer.mozilla.org/en/docs/Web/CSS/Value_definition_syntax#Keywords):
`auto`, `smaller`, `ease-in`
* [Единицы измерения](https://developer.mozilla.org/en/docs/Web/CSS/length):
    * [Абсолютные](https://developer.mozilla.org/en/docs/Web/CSS/length#Absolute_length_units): `px`, `cm`, `pt`
    * [Относительные](https://developer.mozilla.org/en/docs/Web/CSS/length#Relative_length_units): `em`, `rem`, `%`
* [Строки](https://developer.mozilla.org/en/docs/Web/CSS/string): `"image.png"`, `'image.png'`
* [Адреса](https://developer.mozilla.org/en-US/docs/Web/CSS/url): `url("image.png")`, `url(image.png)`
* [Цвета](https://developer.mozilla.org/en/docs/Web/CSS/color): `#00ff00`, `rgba(34, 12, 64, 0.3)`

#HSLIDE

### CSS: [сокращенные свойства](https://developer.mozilla.org/en-US/docs/Web/CSS/Shorthand_properties)

```css
border-width: 1px;
border-style: solid;
border-color: #000;
border: 1px solid #000;
```

[Пример](https://jsfiddle.net/sergdenisov/psjq6k5L/).

#HSLIDE

### CSS: [синтаксис](https://developer.mozilla.org/en-US/docs/Web/CSS/Syntax) (2)

![CSS Syntax: Ruleset](images/css-syntax-ruleset.png)

#VSLIDE

![CSS Syntax: Statements](images/css-syntax-statements.png)

#HSLIDE

### CSS: [@import](https://developer.mozilla.org/en-US/docs/Web/CSS/@import) и [@media](https://developer.mozilla.org/en-US/docs/Web/CSS/@media)

```css
@import url("fineprint.css") print;
@import url('custom.css');
@import 'land.css' (orientation: landscape);
```

[Пример](https://jsfiddle.net/sergdenisov/upkjzhys/):

```css
@media (max-width: 500px) {
    div {
        color: red;
    }
}
```

#HSLIDE

### CSS: [display](https://developer.mozilla.org/en-US/docs/Web/CSS/display)

[Пример](https://jsfiddle.net/sergdenisov/2m3umd53/):

```css
display: none;
display: inline;
display: block;
display: inline-block;
display: list-item;
display: table;
display: table-cell;
```

#HSLIDE

### CSS: [поток документа](https://developer.mozilla.org/en-US/docs/Web/CSS/Visual_formatting_model)

* [Блочные элементы](https://developer.mozilla.org/en-US/docs/Web/CSS/Visual_formatting_model#Block-level_elements_and_block_boxes)
располагаются друг за другом вертикально.
* [Строчные элементы](https://developer.mozilla.org/en-US/docs/Web/CSS/Visual_formatting_model#Inline-level_elements_and_inline_boxes)
располагаются друг за другом горизонтально и построчно.

#HSLIDE

### CSS: [блочная модель](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model)

![CSS: Box model](images/boxmodel.png)

#VSLIDE

* [width](https://developer.mozilla.org/en-US/docs/Web/CSS/width)

* [height](https://developer.mozilla.org/en-US/docs/Web/CSS/height)

* [line-height](https://developer.mozilla.org/en-US/docs/Web/CSS/line-height)

* [padding](https://developer.mozilla.org/en-US/docs/Web/CSS/padding)

* [border](https://developer.mozilla.org/en-US/docs/Web/CSS/border)

* [box-sizing](https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing)

* [margin](https://developer.mozilla.org/en-US/docs/Web/CSS/margin)

[Пример](https://jsfiddle.net/sergdenisov/56mb5b7f/).

#HSLIDE

### CSS: [схлопывающиеся `margin`](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing)

![CSS: Margin collapsing](images/collapsing-margins-in-css.png)

#VSLIDE

Только вертикальные `margin` у:

* [Соседних элементов](https://jsfiddle.net/sergdenisov/q3r98cpe/).

* [Родительского и первого/последнего дочернего элеменов](https://jsfiddle.net/sergdenisov/z3szt88k/).

* [Пустого элемента](https://jsfiddle.net/sergdenisov/d79o4g9b/).

#HSLIDE

### CSS: [float](https://developer.mozilla.org/en-US/docs/Web/CSS/float)/[clear](https://developer.mozilla.org/en-US/docs/Web/CSS/clear)

![CSS: Float/Clear](images/directionalclearing.png)

#VSLIDE

```css
float: left;
float: right;
float: none;
clear: left;
clear: right;
clear: both;
clear: none;
```

[Пример с left](https://jsfiddle.net/sergdenisov/zzwvuk1z/1/),
[пример с right](https://jsfiddle.net/sergdenisov/50g0tkoj/1/),
[пример с both](https://jsfiddle.net/sergdenisov/jLm6k2Lu/).

#HSLIDE

### CSS: [position](https://developer.mozilla.org/en/docs/Web/CSS/position)

```css
position: static;
position: relative;
position: absolute;
position: fixed;
```

* [Пример с relative](https://jsfiddle.net/sergdenisov/o4r4nbam/).
* [Пример с absolute](https://jsfiddle.net/sergdenisov/59vapgdm/).
* [Пример с fixed](https://jsfiddle.net/sergdenisov/zgswLmrk/).

#HSLIDE

### CSS: [контект наложения](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index/The_stacking_context)<br/>и [z-index](https://developer.mozilla.org/en/docs/Web/CSS/z-index)

<img style="float: right;" src="images/understanding_zindex.png" alt="CSS: z-index">

* Root
    * DIV&nbsp;#1
    * DIV&nbsp;#2
    * DIV&nbsp;#3
        * DIV&nbsp;#4
        * DIV&nbsp;#5
        * DIV&nbsp;#6

#VSLIDE

Новый контекс создается для:

* Главного элемента `<html>`.

* Элементов с `position: absolute`/`position: relative` с `z-index` отличным от `auto`.

* Элементов с `position: fixed`.

* Элементов с `opacity` меньше 1.

* Элементов с `transform` отличным от `none`.

[Пример](https://jsfiddle.net/sergdenisov/6v8dwtbh/).

#HSLIDE

### CSS: [селекторы](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Selectors)

* [Простые](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Simple_selectors):
по элементам, классам или id.
* [По атрибутам](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Attribute_selectors).
* [По псевдо-классам](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Pseudo-classes_and_pseudo-elements#Pseudo-classes).
* [По псевдо-элементам](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Pseudo-classes_and_pseudo-elements#Pseudo-elements).
* [Комбинаторы](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Combinators_and_multiple_selectors).

#VSLIDE

### Простые селекторы

```css
strong {
    color: red;
}
.key {
    color: green;
}
#principal {
    font-weight: bolder;
}
```

[Пример](https://jsfiddle.net/sergdenisov/5anfbc64/).

#VSLIDE

### Селекторы по атрибутам

```css
[data-vegetable] {
    color: green
}
[data-vegetable="liquid"] {
    background-color: goldenrod;
}
[data-vegetable~="spicy"] {
    color: red;
}
```

[Пример](https://jsfiddle.net/sergdenisov/o5zx0ktg/1/).

#VSLIDE

### Селекторы по псевдо-классам

[Псевдо-классы](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes):
```css
:active, :checked, :disabled, :first-child,
:focus, :hover, :last-child, :visited
```

[Пример](https://jsfiddle.net/sergdenisov/fww3m0s3/).

#VSLIDE

### Селекторы по псевдо-элементам

[Псевдо-элементы](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-elements):

```css
:after, :before, :first-letter, :first-line
```

[Пример](https://jsfiddle.net/sergdenisov/kd9hfb2d/).

#VSLIDE

### Селекторы-комбинаторы

```css
div.red {
    color: red;
}
div p {
    color: green;
}
div > p {
    color: white;
}
div + div {
    color: yellow;
}
div ~ div {
    color: black;
}
```

[Пример](https://jsfiddle.net/sergdenisov/ajpqx908/).


#HSLIDE

### CSS: [наследование](https://developer.mozilla.org/en-US/docs/Web/CSS/inheritance)

* [Наследуемые свойства](https://developer.mozilla.org/en-US/docs/Web/CSS/inheritance#Inherited_properties):

```css
color, cursor, font, line-height, text-align
```

* [Ненаследуемые свойства](https://developer.mozilla.org/en-US/docs/Web/CSS/inheritance#Non-inherited_properties):

```css
border, padding, margin
```

* Значение [inherit](https://developer.mozilla.org/en-US/docs/Web/CSS/inherit):

```css
#sidebar h2 { 
    color: inherit;
}
```

[Пример](https://jsfiddle.net/sergdenisov/5nwy6b19/).


#HSLIDE

### CSS: [каскад](https://developer.mozilla.org/en-US/docs/Web/CSS/Cascade)

&nbsp;| Origin | Importance
------|--------| ----------
1 | user agent | normal
2 | user agent | !important
3 | user | normal
4 | author | normal
5 | CSS Animations |
6 | author | !important
7 | user | !important

#HSLIDE

### CSS: [специфичность](https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity)

Specificity | Selector type | Importance
------------|---------------|-----------
[0001] | Tag/pseudo-element | normal
[0010] | Class/pseudo-class | normal
[0100] | ID | normal
[1000] | Style | normal

#VSLIDE

Specificity | Selector type | Importance
------------|---------------|-----------
[0001 0000] | Tag/pseudo-element | !important
[0010 0000] | Class/pseudo-class | !important
[0100 0000] | ID | !important
[1000 0000] | Style | !important

#HSLIDE

### CSS: рекомендации

* Предпочитайте селекторы по классам остальным.
* Именуйте классы [по смыслу](https://google.github.io/styleguide/htmlcssguide.xml?showone=ID_and_Class_Naming#ID_and_Class_Naming),
а не по значению.
* Старайтесь не использовать [сокращения](https://google.github.io/styleguide/htmlcssguide.xml?showone=ID_and_Class_Name_Style#ID_and_Class_Name_Style).
* Старайтесь избегать [хаков](https://google.github.io/styleguide/htmlcssguide.xml?showone=Hacks#Hacks).
* [Google CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.xml#CSS_Style_Rules).

#HSLIDE

### Ссылки

* [Mozilla Developer Network (MDN)](https://developer.mozilla.org/en/).
* [Can I Use?](http://caniuse.com)
* [Stackoverflow](http://stackoverflow.com) (только с пруфами)

