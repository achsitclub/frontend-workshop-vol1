
html tags always start with <>, with tag name inside it
and end with </> with tag name inside it.
It is same as { and } in c++ or other languages.

example : 
<html> </html>
<head> </head>
<body> </body>
etc!
There are certain tags that must go inside other tags.
These tags are child tags, and tags containing them are Parent tags.

For Example,
<html> tag is parent of all other tags. It must contain all other tags.
        - HTML tag is starting of a HTML document


<meta> tag is used after html tag. 
        - It is used to in Search Engine Ranking
        - It doesnot need to be closed

<head> tag is used just after meta tag
        - It is used for linking to other documents, fonts, css files, etc.
        - It is the parent of title tag
        <title> tag is inside head tag.
            - It is used to give title of a HTML document
        </title>
</head>
 
 
<body> tag is used after head tag.
    - It contains the content of entire web page.
    - Is parent of most tags used in HTML document.
------------------------------------------------
            Typography Tags
------------------------------------------------
    Heading Tag: 
        -h1 to h6 (
            <h1>Heading 1</h1>
            <h2>Heading 2</h2>
            <h3>Heading 3</h3>
            <h4>Heading 4</h4>
            <h5>Heading 5</h5>
            <h6>Heading 6</h6>
        )
------------------------------------------------
    Paragraph Tag
        - p (
            <p> Contains Paragraph.... </p>
        )
------------------------------------------------
    Bold, Italic and Underline Tags:
        - b(
            <b> Bolds Text</b>
        )
        - i (
            <i>Italics any text </i>
        )
        - u (
            <u>Underlines a Text </u>
        )
------------------------------------------------
    Line Break
        - br(
            text goes here <br> Text goes here
            In Browser:

            {
                text goes here
                Text goes here
            }
        )
        -No Closing Required
------------------------------------------------
        font tag
            - font (
                <font>
                    Text Goes here
                </font>
            )
------------------------------------------------
            Link Tags
------------------------------------------------
    Hyperlink
            - a (
                <a href = "refrence-link">Name of Link </a>
            )
            -Can be internal or external
            -Name of link can me text or image
    Document Link
            - link (
                <link rel = "relation of linked document to html" href = "refrence-link">
            )
------------------------------------------------    
                Image Tag
------------------------------------------------

    Image
            - img(
                <img src = "path of image">
            )
            - No closing Required
------------------------------------------------
            Listing Tags
------------------------------------------------

    Listing
            - Ordered List - ol(
                <ol>
                    <li> List Item 1 </li>
                    <li> List Item 2 </li>
                </ol>
            )
            -Unordered List
                <ul>
                    <li> List Item 1 </li>
                    <li> List Item 2 </li>
                </ul>
------------------------------------------------
            Page Division Tags
------------------------------------------------
    division
            - div (
                <div>
                    Content goes here
                </div>
            )
            - Used to divide page in certain parts
            - Can contain any tags in between
            -Extremely Useful for Efficiency, Code Redability, Debugging
------------------------------------------------
    Header 
        - header (
            <header>
                Content goes here
            </header>
        )
        - Used to wrap Content that denote starting of html page.
------------------------------------------------
    Navigation
            - nav (
                <nav>
                    Content goes here
                </nav>
            )
            - Used for Wrapping Navigation Link Items
            - Typically used inside Header tag, but can be used anywhere (even independently)
------------------------------------------------
    Section
            - section (
                <section>
                    Content goes here
                </section>
            )
            - same as div
            - More Redable and understandable
------------------------------------------------
    Aside
            - aside (
                <aside>
                    Cintent goes here
                </aside>
            )
            -Same as section
            - Used to Differentiate the content that goes 
              in side bar with conntent on main part of page
------------------------------------------------
    Footer
            - footer (
                <footer>
                    Content Goes Here
                </footer>
            )
            - Same as Header, but for denoting ending of HTML
            
------------------------------------------------

</body>
------------------------------------------------
            Script Tags
------------------------------------------------
        Internal Script
            - script(
                <script>
                    Script Language Here
                </script
            )
        - External Script
            - script (
                <script src="path for script file"></script>
            )
</html>
