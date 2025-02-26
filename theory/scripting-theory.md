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
    * E.g.: name="viewport", content="width=device-width, initial-scale=1.0"
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
    Purpose: Used for adding side bars


#### <section>...</section>


#### <nav>...</nav>
    Purpose: Used for navigation links


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
    - loading - "lazy", to defer the loading of an image (or other media content) until it is actually needed on the page.  This can improve page load performance by reducing the initial amount of data that needs to be loaded when the page is first accessed.


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
* <th> tag - this tag is used to create a heading inside the <thead> tag
* <td> tag
    - to give cell data (called table data)
    - Property: 
        - rowspan: to expand a cell into multiple rows
        - colspan: to expand a cell into mulitple cols
* <thead> tag
    - to define table header section
    - in general, defined for first row of the table
* <tfoot> tag
    - to define table footer section
    - in general, this row will have summary we define the table (like sum)

* <tbody> tag
    - to define table body section
    - in general, all the content except header tag goes to this tag

Note: <thead>, <tfoot>, and <tbody> - only used when we want to implement a style to a group of rows


#### <form>...</form>
* Purpose: to collect user input as data
* it uses following tags:
    ##### <input>...</input>
    * attributes: 
        - 'value': text that appears on the input field (e.g., text on the button). 'value' attribute in text fields represent default value of the input. It is not the faded example we see in text bars.
        - 'type' : it defines type of input (like, button, checkbox, radiobutton, etc.)
        - 'placeholder' - example text in the text field for the user understanding
    * input can be taken in following forms:
        - text: text-box
        - button
        - checkbox
        - color: color selector
        - radio: radio-button
            - 'name' attribute connects all radio-buttons together so that only one out of them can be selected
            - 'id' attribute helps to connect to 'label'
        - date: date-picker
        - datetime-local
        - Specific fields:
            - email
            - password
            - month
            - time
            - week
            - number: generally used for counter
            - range
            - url
            - tel: telephone
            - search
        - submit:
            - there are two ways to send the data collected in form to server:
                1. submit button
                2. <form action=""> - 'action' attribute in form button
        - reset
        - file: file-selector (from local system, etc.)
        - image: image as buttons
        - hidden: ?
        
    ##### <label>...</label>
    * used to create labels
    * used by screen readers
    * attributes: 
        - 'for': its value is same as value if 'id' attribute of <input>. This links these two tags.
    
    ##### <select>...</select>
    * used to insert a drop down menu for the user to select
    * <option value="item1">item to display</option> tag is used to create options of the drop-down menu
    * The options should be enclosed inside the <select> tag.
    * Attribute - 'multiple' enables to select multiple options from the drop-down
    
    ##### <button>...</button>
    
    <textArea>
    * used to take multiple line input from user
    * Attributes: 
        - id
        - cols: to define width of the textarea
        - rows: to define length of the textarea
        - placeholder


#### <details>...</details>
    * Purpose: To create collapsible section of content that can be toggled by the user
    * Syntax: 
    <details>
        <summary>Click to view more details</summary>
        <p><!-- This is additional content that is hidden initially and can be revealed by clicking the summary above --></p>
    </details>


#### <audio>...</audio>
    * Purpose: To add audio on the webpage
    * Refer: project1.html
    * Syntax:
        <audio controls>
            <source src="<location-of-audio-in-project>" type="audio/ogg">
            name-of-the-file
        </audio>
    * Attributes: 
        - controls: to have controls on the screen
        - <source> tag: separate tag included to add src of the file.
        Note: we can directly add 'src' attribute to the <video> to define file location


#### <video>...</video>
    * Purpose: To add video on the webpage
    * Refer: project1.html
    * Syntax: 
        <video width="320" height="240" controls>
            <source src="<location-of-audio-in-project>" type="video/mp4">
            name-of-the-file
        </video>
    * Attributes: 
        - controls: to have controls on the screen
        - <source> tag: separate tag included to add src of the file.
        Note: we can directly add 'src' attribute to the <video> to define file location

#### <iframe>...</iframe>
    * Purpose: It is 'inline frame' tag, used for adding maps, code rendering sandbox, youtube-videos, other webpages, etc.
    * Refer: project1.html
    * Syntax: 
        <iframe
            id="inlineFrameExample"
            title="Inline Frame Example"
            width="300"
            height="200"
            src="https://www.openstreetmap.org/export/embed.html?bbox=-0.004017949104309083%2C51.47612752641776%2C0.00030577182769775396%2C51.478569861898606&amp;layer=mapnik">

        </iframe>
    * Attributes: 
        - src="<exact link of the item to render on your webpage>"
    * Notes: 
    Rendering youtube videos in iframe has a format
    E.g.: 
    - May not work src="https://www.youtube.com/watch?v=k7ELO356Npo&t=17828s"
    - Will work when = "https://www.youtube.com/embed/k7ELO356Npo&t=17828s"
    - Adding autoplay for any video (project3) = "https://www.youtube.com/embed/k7ELO356Npo?autoplay=1&mute=1"

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
    * used to combine section of related items inside a box (appears on UI)
    * E.g.: following radiobuttons are related and can be combined into a fieldset:
        male
        female
        other
    * <legend>: to provide captions to a fieldset (appears as a description to the fieldset on UI)

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

#### span tag
* this is inline tag and takes space as needed and starts from same line
* 

#### <audio>...</audio>

#### <video>...</video>



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
5. div tag
    - non-semantic tag (i.e., doesn't provide any meaning to the script)
    - stands for 'division tag'
    - used for creating divisions and used as a wrapping container
    - now the wrap can be used to define properties on the contents together
    - it is a block element and takes up complete line space
6. Elements:
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