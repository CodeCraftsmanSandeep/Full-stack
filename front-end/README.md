
| Stuff | What is does? | Similar to: | Who needs full forms? :-( | Brief note | More brief note |
|:--|:--|:--|:---|:--|:---|
| HTML | Structure | Skeleton | Hyper Text Markup Language | specify the web page content and its structure. | Noun | 
| CSS  | Styling | Skin | Cascading Style Sheets | specify styling and layout information. | Adjective |
| JS | Functionality | Brain | Java Script | specify the behavior of interactive parts of the web page. | Verb |

----
### Notes
#### HTML
- HTML is case-insensitive
- HTML is a forgiving markup language, it does not give any errors (or) feedback
- We can of course customize images using CSS, but now a days it is recommended practise to include width and height info in html because the browser will be able to use this info.
- You can use placeholder images when developing HTML code: https://placehold.co/
- Semantic:
    - Semantic HTML refers to using HTML tags that convey meaning about the content both to the browser and to humans (developers, screen readers, SEO). Use semantic elements as much as possible
        - like: `main` | `header` | `section` | `article`
    - The following have no semantic meaning in html
        - like: ```div``` | ```span``` | ```b``` | ```i``` | ```br```
- Buttons always behave the same whether you use a `<button>` element or an `<input>` element.
- CMS: Content management system
    - Examples: WordPress
- "\" : means pointing to root
- `div` and `section`
    - If there is no semantic tag that you can use, only then use `div`. `div` is generic container for layout and styling.
    - Use `section` when you want to group related content with semantic meaning, especially if it has a heading. 
- there are many icons on https://fontawesome.com/ to use
- icons and images in https://undraw.co/

| Syntax / Term | Sweet note 📝 |
|:--|:--|
| ```<hr>``` | Horizontal line |
| ```<h1> <\h1>``` to ```<h6> <\h6>``` | Headings + Semantic meaning (for SEO) + Organisation of content | 
| ``` <p> <\p>``` | Paragraph
| ``` <em> <\em>``` | Emphasize |
| - ordered lists ```<ol> <\ol>``` <br> - unordered lists ```<ul> <\ul>``` <br> - definition lists `<dl>` which works with definition term `dt` and definition description `dd` | Lists |
| ``` <strong> <\strong> ``` | Importance (has semantic meaning) |
| ``` <br> ``` | Break line |
| `<a><\a>` | Anchor tag: to link |
| [HTML character codes](https://html.spec.whatwg.org/multipage/named-characters.html#named-character-references) | like ```&nbsp``` |
| ``` <address> <\address> ``` | Address |
| ``` <abbr> <\abbr> ``` | Abbrevation |
| Referencing (or) Linking | We will have two types: i) relative ii) absolute <br> We can link to external links (or) files on same server (or) to content in same page (basically internal link)|
| ```<nav> </nav>``` | Navigation bar |
| ```<img>``` | Image (lazy (or) eager loading) |
| `<figure> </figure>`| |
| ```header``` | Top section of a page or article |
| ```main``` | main content area |
| ```<time> </time>``` | Time semantic meaning |
| ```<form> </form>``` | Form stuff <br> -text -number -email -password -tel -checkbox -select -radiobuttons -button -submitbutton -textarea -file -time -year -week -month -range -color -date -datetime -url and what not? <br> - **form validation:** checking whether the input entered is valid or not|
| ```<fieldset> </fieldset>``` | Grouping widgets in form |
| ```<legend> </legend>``` | Title of the form |
| **inline elements** | - not creating a new line (like `a`, `em`, ```strong```) <br> - dont take full width <br> - can contain inline elements | 
| **block level elements** | - like ```h1``` (or) ```p``` (or) `div`, they give line breaks <br> - block level elements take full width <br> - can contain both inline and block level elements |
| Whitespace collapsing | spaces in code are ignored |
| ```<span> </span>```  | - generic inline container <br> - No semantic meaning <br> - used for grouping (or) targeting |
| ```<button> </button>``` | - You want button? then use this |
| `<progress> </progress>` | progress bar |
| `<meter> </meter>` | meter |
| `blockquote` | block of text that is quoted from another source | 
| `pre` | preformatted text | 
| `cite` | Doing everything by yourself is useless, cite some stuff | 
| `bdo` | override the text direction | 
| `q` | quote | 
| `u` | underline |
| `<b> </b>` | Just bold. No semantic meaning. | 
| `small` | small |
| `del` | deleted text | 
| `ins` | inserted text | 
| `sub` | subscript |
| `sup` | superscript | 
| `audio` `video` `controls` `source` `iframe` | media stuff | 
| `nav` | - internal navigation: can be used when the page is long (or) it is single page web application <br> - external navigation: when navigating to another page | 
| `table` `thead` `tbody` `tr` `td` | I love tables |
| `download` | attribute for downloading |
| `mailto` `tel` | to directly send email (or) make phone call | 


------
#### CSS

- different ways to use CSS
    - inline css is not the best practise because:
        - it combines html and css at once place making it difficult to maintain and read
        - resuability is less compared to internal and external css
    - internal css has less resuability than external css
    - priority of applying: (see this [code](./17_css/index.html))
        1) Inline CSS
        2) ID selector
        3) Class
        4) Element selector
        5) If two rules have the same strength then one which is written later applys (basically the later it is, it can win)
    - Cascading is the process the browser uses to decide which CSS rule applies when there are multiple conflicting rules for the same element.    
        - `!important` is used to overwrite the normal existing rules
- `box-shadow`

---
- Few useful examples:
    | Selector             | Matches                                              | Specificity              |
    | -------------------- | ---------------------------------------------------- | ------------------------ |
    | `*` (universal)      | All elements                                         | 0-0-0                    |
    | `:where(...)`        | Whatever is inside                                   | 0-0-0                    |
    | `element` (e.g. `p`) | Elements by tag                                      | 0-0-1                    |
    | `.class`             | Elements by class                                    | 0-1-0                    |
    | `[attr]`             | Elements with attribute                              | 0-1-0                    |
    | `:hover`             | Elements in hover state                              | 0-1-0                    |
    | `#id`                | Element with that ID                                 | 1-0-0                    |
    | Inline style         | Element style attribute                              | 1-0-0-0 (highest normal) |
    | `!important`         | Overrides everything (not specificity, but priority) | —                        |

---

| Stuff | Description | 
|:---|:---|
| Types of adding CSS: | 1) Internal CSS <br> 2) External CSS <br> 3) In-line CSS |
| shortand properties | like `padding: 10px 15px 15px 5px;`, basically top right bottom left|
| ```calc()``` | Allow calculations |
| `rotate()` | | 
| `@rules()` | - media query `@media` |
| `line-height` | Controls the vertical spacing between lines of text |
| `text-transform` `text-align` `font-weight` | |
| `color` `padding` | good stuff |
| `*` | universal selector |
| `#` | id selector |
| `.` | class selector |
| `[attr = value] {}` | attribute selectors | 
| `>` | direct descandant styling |
| box-model | - content <br> - border <br> - padding: space between content and border <br> - margin: space outside border <br> ----- <br> `box-sizing` property: <br> - `content-box` <br> - `border-box` |
| `specificity` | is a set of rules in CSS that determines which style declarations are applied to an element where there are multiple, potentially conflicting rules |
| pseudo elements <br> - `::first-line` <br> - `::first-letter` | is a keyword that can be added to a selector that lets you style a specific part of the selected element(s) |
| pseudo class <br> - `:hover` | lets you style a specifi state of the selected element(s) |
| position | - absolute <br> - relative <br> - fixed <br> - sticky <br> - static | 
| font sizes | - `1em` : element's own font size <br> - `1rem` : root font size | 
| flexbox | - main axis <br> - cross axis <br> - `flexbox` <br> - flex container <br> - flex items <br> - `flex-grow` <br> - `flex-shrink` <br> - `flex-basis` <br> - `flex-direction` is important |
| 1 vh | 1% of the height of the browser window (viewport) | 


------
## notes
- dependencies for styling in web forms https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Forms/Styling_web_forms 
- need of CSS: https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics