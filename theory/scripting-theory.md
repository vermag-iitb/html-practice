# Tags
1. it is a markup entity to provide contenr (e.g., video, audio, etc.) struture, semantics and formatting.
2. it is a keyword with <>
3. it instructs browser and hence also identified as a pre-defined program (or function)
4. Tags have attributes to add some effects
5. Types: 
- paired: <>...</>
- unpaired (or bodyless tags): <---/> 
    * E.g.: <br/>, <img.../>, <link.../>

#### <!Doctype HTML> - Boiler plate code
* defines version section for HTML5 and above
* stands for documentation type
* doctype = DOCTYPE (recommended)
* For HTML4 and below, <!Doctype html version-url>
* Public Urls: 
    - "-//w3c//DTD HTML 4.0/EN"
    - http.//www.w3c.org/TR/html4/strict.dtd
    Here, strict.dtd - is a file which contains what tags are present in HTML4.0 and their definition.
    Same urls are used for below versions as well with version corrected to 3,2, or 1
* W3Cs guidelines are suggestions and not restrictions and hence, we can skip any part of it.
* Shorthand: !+tab


## Structure tags

#### <html>...<!html>
* Note: 
    * initmates that webpage designing is started and closed between these tags.
    * Attributes:
        - lang='en' 


#### <head>...<!head>
* Note: 
    * this executes first
    * it stores metadata (<meta> 
        defining website which appears as description on google), seo data, and website title (<title>) data

##### <meta attr = "" attr = "" .../>
    * attribute: name, content, property, http-equiv, charset
    * E.g.: name = title, description, keywords, author, copyright, robots
    * E.g.: name="viewport" content="width=device-width, initial-scale=1.0"
    * E.g.: property = og:type, og:url
    * E.g.: charset="UTF-8"
    * E.g.: http-equiv="X-UA-Compatible" content="IE=edge"


#### <body>...<!body>
* Note: 
    * it gets executed after <head> tag
    * it consists of design code with individual elements of the webpage as separate labels


#### <title>...</title>
* defined for each web-page
* generally used inside <head>...</head>


#### <header>...</header>


#### <footer>...</footer>


#### <main>...</main>


#### <article>...</article>


#### <aside>...</aside>


#### <section>...</section>


#### <nav>...</nav>



## Semantic tags

#### Paragraph tag
* <p>...</p>


#### <link>...</link>
* used to set icons, hyperlinks, logos, etc.
* E.g.: <link rel="icon" href="filename"/>
    - rel - stands for relative
* supported images - .jpg, .bmp, .png, .gif, .tif, .ico (photoshop)
* preferrable image size - 18px18px, 20x20px
* logo comes to all webpages by default


#### <a>...</a>
* called anchor tag as it anchors to a particular destination
* used for hyperlinks to text, image, servlet, asp.net, php, node, audio, etc.
* hyperlinks helps to navigate on the webpage or to different webpage
* Identified by blue color, under line, and hand pointer while hovering on text
* Syntax: <a attributes>Display text</a>
* Attributes: 
    - href = url or directory path of the item to be anchored
    - target = "_self" (default value, to locate same tab)
             = "_blank" (new and blank tab)
             = parent (single webpage partitions/blocks)
             = framename (in a block of webpage, used when the webpage is divided into multiple blocks)
* Note: if the file doesn't open, then browser forces to download by default
* Note: <a href = "#element_id">text</a> -> to navigate on same page using links for headings


#### Heading tag
* <h1>...</h1>
* <h2>...</h2>
* <h3>...</h3>
* <h4>...</h4>
* <h5>...</h5>
* <h6>...</h6>
Note: 
1. Difference between different headings is not about size and appearance. However, difference lies in semantics (i.e., priority is more for H1 than H2). Also, the appearance can be changed as needed later for H1 to H6.
2. <h7> or anything similar will behave like normal text in <p> tag. 


#### <img>...</img>
* used to display image on webpages
* Syntax: <img attributes/>
* Place all images in the same folder or create a subfolder called 'images' for auto-pick up
* Extensions: .jfif, .svg, .jpg, .bmp, .gif, .tif, .png, .webp, etc.
* Mostly all images are supported. Limitations were for icon images
* Attributes: 
    - src - source address of the image
    - width - width of image
    - height 
    - title - info. displayed when mouse pointer hovers on the image
    - alt - alternative text, this text appears in place of image if it doesn't load


#### List tags
    * ol - ordered list (it is block level tag and paired tag)
        - used to display text as list
        - possible bullets =? 1, A, a, i (roman), I(roman)
        - After single alphbets are finished, double alphabets start (AA, AB, AC, etc.)
        - attributes: 
            - type='A (to define capital letters as bullets)
            - start="1001" (to define desirable point to start)
            - reversed (to print reverse alphabets/numbers), hence 'start' attribute is mandatory here
    * li - list tag (it is block level tag and paired tag)
        - defines one element of the list
        - without <ol> tag, <li> tag will give 'dot' as bullet as default
        - with <ol> tag, <li> tag will give '1' as bullet as default
    * syntax: 
        <ol attr>
            <li> text </li>
            <li> text </li>
        </ol>
    * Nested list syntax: 
        <ol>
            <ol attr>
                <li> text </li>
                <li> text </li>
            </ol>
            <ol attr>
                <li> text </li>
                <li> text </li>
            </ol>
        </ol>
    * ul - unordered list
        - supported for dot, circle, square, etc.
        - syntax is similar to 'ol'
        - attribute: type="dot"
    
* Note: Difference between ordered and unordered list is about the importance to their sequence, and not the bullets they appear with.


#### Table tags
* Syntax: 
    <table>
        <tr> 
    </table>
* <table> tag itself is not responsible to generate a table. It is to confine rows and column tags and attributes.
* <tr> tag - to draw one row (table row)
* <th> tag - to draw one column
* <td> tag - to give cell data (called table data)
* <thead> tag - to define table header section
* <tfoot> tag - to define table footer section
* <tbody> tag - to define table body section
Note: <thead>, <tfoot>, and <tbody> - only used when we want to implement a style to a group of rows


#### <form>...</form>


#### <input>...</input>



## Formatting tag
Note: Formatting tags are generally not used, as CSS is used for styling the content.
* <strong> - bold text (<b> - bold tag - deprecated)
* <u> - underline
* <i> - italics (deprecated)
* <em> - italics (15%) - emphasize
* <s> - strikeout
* <sub> - subscript
* <super> - superscript
* <pre> - Instead of writing <br/> tag everywhere, we can directly use <pre> tag, which picks text in form as presented in html file.
* <code> - 


## Other tags


#### <legend> text </legend>
* to define name and heading for a box or its sub-parts

#### Fieldset tag
    * Used to draw line/border around multiple elements or block of tag
    * any number of borders can be drawn
    * Paired and block level tag
    * Syntax: 
        <fieldset attr>
            <legend> text </legend>
            {
                block of tages
            }
        </fieldset>
    * E.g.: 
        <fieldset style = "border:5px; solid red; width:900px; text-align:center;text-size:166px; text-family:Tahoma;">
            <legend> My-UI-skills </legend>
            <ol>
                <li> HTML </li>
                <li> CSS </li>
                <li> JS </li>
            </ol>
        </fieldset>

#### class tag
    to help combine elements in html script to be able to apply editing together

##### id attribute:
    to identify every element in html script as individual

#### div tag
* non-semantic tag (i.e., doesn't provide any meaning to the script)
* stands for 'division tag'
* used for creating divisions and used as a wrapping container
* now the wrap can be used to define properties on the contents together
* it is a block element and takes up complete line space

#### span tag
* this is inline tag and takes space as needed and starts from same line
* 

#### <button>...</button>

#### <label>...</label>

#### <span>...</span>

#### <table>...</table>

#### <audio>...</audio>

#### <video>...</video>

#### <section>...</section>




## Other useful content:
1. <!--comment-->
2. <br> or </br> - line break
3. Entities - used to print operators icon webpage 
    - &entity; - 100 entities written in english
    - &#operator; - 300 operators, written in hexadecimal no. of symbols
4. Attributes: 
    - special features/settings/properties of a tag
    - Syntax: <tag-name attribute="parameter" attribute2="parameter2" ...>
    - "", '', no-quotes - all work as same
    - Types of attributes:
        1. Global attributes: 
            - E.g: id, name, class, style, align, width, height, title, etc.
            - They are used for multiple commonly used tags
        2. Specific attributes: 
            - these are specific to some tags
            - E.g: rel, href, colspan, rowspan, action, alt, src, etc.
        3. Event attributes: 
            - specific for Javascript only
            - 'on' - precedes all these attributes
            - E.g.: onclick, onload, onfocus, onblur, onchange, onsubmit, onkeypress, etc.
        4. Optional attributes: 
            - introduced in html5
            - E.g.: lang, type, etc.
5. Elements:
    * Block elements
        - always get created in next line
        - take all the horizontal space on the webpage
        - can be converted to inline by using style attr with property: "display: inline"

    * Inline elements
        - don't come in next line
        - take space as required by the content


# ShortHands in VS-Code
1. Boiler plate code - !+TAB/ENTER
2. Run in browser via Live Server - 
    - 'Go Live' button in right corner
    - Rt. Click + Open with Live Server
3. 