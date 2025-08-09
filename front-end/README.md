
| | | 
|:--|:--|
| HTML | Structure |
| CSS  | Styling   |
| JSS  | Functionality |

--
### Notes
#### HTML

- We can ofcourse customize images using CSS, but now a days it is recommended practise to include width and height info in html because the browser will be able to use this info.
- You can use placeholder images when developing HTML code: https://placehold.co/
- Semantic:
    - Semantic HTML refers to using HTML tags that convey meaning about the content both to the browser and to humans (developers, screen readers, SEO). Use semantic elements as much as possible
        -  ```main```
        - ```header```
        - ```section```
        - ```article```
    - The following have no semantic meaning in html
        - ```<div>```
        - ```<span>```
        - ```<b>```
        - ```<i>```
        - ```<br>```
- forms:
    - **form validation:** checking whether the input entered is valid or not

| Syntax / Term | Sweet note 📝 |
|:--|:--|
| ```<hr>``` | Horizontal line |
| ```<h1> <\h1>``` to ```<h6> <\h6>``` | Headings + Semantic meaning (for SEO) + Organisation of content | 
| ```html 
<a><\a> 
``` | Anchor tag: to link |
| ``` <p> <\p>``` | Paragraph
| ``` <em> <\em>``` | Emphasize |
| ``` <strong> <\strong> ``` | Importance |
| ``` <br> ``` | Break line |
| [HTML character codes](https://html.spec.whatwg.org/multipage/named-characters.html#named-character-references) | like ```&nbsp``` |
| ``` <address> <\address> ``` | Address |
| ``` <abbr> <\abbr> ``` | Abbrevation |
| - ordered lists ```<ol> <\ol>``` <br> - unordered lists ```<ul> <\ul>``` <br> - descriptive lists ```<dl> <\dl>``` | Lists |
| Referencing (or) Linking | We will have two types: i) relative ii) absolute <br> We can link to external links (or) files on same server (or) to content in same page (basically internal link)|
| ```<nav> </nav>``` | Navigation bar |
| ```<img>``` | Image (lazy (or) eager loading) |
| ```figure``` | |
| ```header``` | Top section of a page or article |
| ```main``` | main content area |
| ```<time> </time>``` | |
| ```<time> </time>``` | Time semantic meaning |
| ```<form> </form>``` | Form stuff |
| ```<fieldset> </fieldset>``` | Grouping widgets in form |
| ```<legend> </legend>``` | Title of the form |
| Elements |     - inline elements: not creating a new line (like ```em```, ```strong```) <br> - block level elements: like ```h1``` (or) ```p```, they give line breaks |
| Whitespace collapsing | spaces in code are ignored |
