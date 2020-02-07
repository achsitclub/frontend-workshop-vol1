CSS or Cascading Style Sheet describes how HTML elements should be displayed in Browser Screen.
The Layout of css is as follows: 

selectorType SelectorName{
    css Properties;
}
-> Semicolon is used to represent end of one property and its value.
-> CSS is a top Down Approach
    It means, the is the same element has been styled at top has been styled 
    differently later in the css document, the late properties are applied 
    while rendering.

-> A dot '.' is used for Selecting Class name of html
example
    HTML:
        <div class="className1">
            content here
        </div>

    CSS:
        .className1{
            CSS properties here
        }
-> A hash '#' is used for selecting ID name of HTML 
    <div id="idName1">
            content here
        </div>

    CSS:
        #idName1{
            CSS properties here
        }
-> No operator selects a valid Tag of html
    Html:
        <div>
            Content Here
        </div>
    CSS:
        div{
            css property Here
        }
->

-----------------------------------------
            Typography
-----------------------------------------

    -Color Properties:

        - Changes Color of Text in CSS
        - Syntax: 
            color: Color Name / rgb value / hex value / hsl value

        - {
            Color: red;
        }
        html:
            <p>
                Hello I am Suparth
            </p>

        CSS:
            p{
                color:red;
            }

    - Font Properties
        - For Styling Font
        - includes various Types
        - Frequently Used:
            - font-family, font-size, font-weight, font-style
            Example:
            html:
                <p class="arialFont">
                    This is Arial Font
                </p>

                <p class="threePxFont">
                    This is 3px Small Font Size
                </p>

                <p class="boldFont">
                    This is Bold Font
                </p>

                <p class="italicFont">
                    This is Italic Font
                </p>
            

            CSS:
                .arialFont{
                    font-family:'Arial',sans-serif;
                }
                .threePxFont{
                    font-size:3px;
                }
                .boldFont{
                    font-weight:bold;
                }
                .italicFont{
                    font-style: italic;
                }
    - Text properties:
        - Used for decoration of text
        - has various variations: text-decoration, text-transform

        Example:
            html:
                <p class="underlineText">
                    This is underlined text
                </p>
                <p class="uppercaseText">
                    this text is uppercased
                </p>
            CSS:
                .underlineText{
                    text-decoration:underline;
                }
                .uppercaseText{
                    text-transform:uppercase;
                }
    - Letter Spacing:
        - Spacing between Letters:
            HTML: 
                <h1>
                    This Text has More Letter Spacing
                </h1>
            CSS:
                h1{
                    letter-spacing:3px;
                }
-----------------------------------------------------------
                Width and Height
-----------------------------------------------------------
    -> Give Certain Width and Height to Element
    -> Syntax:
        width: <amount of width>
        height: <amount of height>

-----------------------------------------------------------
                        Border
-----------------------------------------------------------
    - Give certain border to any element on browser window
    - Syntax:
        border:<amount of pixels> <type of border> <color of border>
            Example:
                a{
                    border:1px solid red;
                }
                or 
                a{
                    border:1px dashed red;
                }


-------------------------------------------------------------------
                            Background
-------------------------------------------------------------------


-> Give background color or image to any div
    - Color can be in pre defined keyword
                 in HEX value
                 in rgb format
                 in hsl format
    
        Syntax:
            background-color: black;
            or 
            background-color:#2a2a2a;
            or
            background-color:rgb(42,42,42);
            or
            background-color: hsl(210,255,100);

        Example:
            
            div{
                background-color:black;
            }

-> Image is defined by giving path to it
    (relative or absolute path)
    (relative path is preferred)

    syntax:
        background-image:url('relative or absolute path to image');
    Example:
        div{
            background-image:url('../img//background.jpg');
        }

    Variations of background image for responsiveness and better positioning on screen

    -> Background-Size:
        -> Size of Background in the division
        syntax:
            background-size: <amount of size of background image in html element>
        
            amount can be in % value or certain keywords

            Keywords:
                cover
                    -> background-size: cover;
                    -> Used to cover the html element. Changes in size when Screen Size Changes
                
                contain
                    -> background-size: contain;
                    -> contains image in a perticular html element
                
    
    -> Background-Position
        -> Position of background in html element
        Syntax: 
        background-position: <size of background image in html element>
             amount can be in % value or certain keywords

            Keywords:
                right
                    -> background-position: right;
                    -> Position the image at its right size being dominant
                
                center
                    -> background-position: center;
                    -> Position the image at its right size being dominant

                 left
                    -> background-position: left;
                    -> Position the image at its right size being dominant

    -> Background-repeat
        -> Repeating or not repeating the background image in html element
        -> Used Keywords:
            repeat
            no-repeat
        Syntax: 
            background-repeat: repat or no-repeat;

    -> Background-attachment
        -> Attaching the element to the html element
        -> Syntax:
            background-attachment: <attachment keyword>

            Keywords:
                -> scroll: Default. Image scrolls with the viewport.
                -> fixed: Fixed background image to element, that is image stays still while everything scrolls
                -> Local: Background image with scroll with html contents

    Example:
            .landingBackground{
                background-image: url('img/backgroung.jpg');
                background-size:cover;
                background-repeat: no-repeat;
                background-attachment:fixed;
            }

    -Linear Gradient: 
        -> Used as a value for background image
        -> Uses 3 parameters: angle of gradient, color value 1, color value 2 
        Syntax: 
        -> background-image: linear-gradient(45deg,blue,red);

        Angle can also be keywords: 
            - to right, to top, to left, to bottom
    

-------------------------------------------------------------
                        Margin and Padding
-------------------------------------------------------------

    Margin: Space outside the border of element
    Padding: Space inside the border of element

    Margin:
        Syntax: margin: <amount of margin>
    Padding: 
        Syntax: padding: <amount of padding>
    
    There are variations in Margin and padding

        Margin:
            Combined Margin:
                margin: <amount of margin from all side>

            Specific Margins:
                margin-top: <amount of margin from top side>
                margin-right: <amount of margin from right side>
                margin-bottom: <amount of margin from bottom side>
                margin-left: <amount of margin from left side>

            Collective Margin:
                margin: <amount of margin from top side> 
                        <amount of margin from right side> 
                        <amount of margin from bottom side> 
                        <amount of margin from left side>

            Paired Margin:
                margin: <amount of margin from top and bottom side>
                        <amount of margin from right and left side>

        Padding : same as margin's variations, with padding keyword except margin



    Example:
    /*Combined Margin*/
    div{
        margin: 10px; /*10px margin from all side*/
    }
    
    /*Specific Margin*/
    div{
        margin-top: 10px; /*10px margin from top side*/
        margin-right: 20px; /*20px margin from right side*/
        margin-bottom: 30px; /*30px margin from bottom side*/
        margin-left: 40px; /*40px margin from left side*/
        
    }

    /*Collective Margin*/
    div{
        margin: 10px 20px 30px 40px ; /*10px margin from top side
                                        20px margin from right side
                                        30px margin from bottom side
                                        40px margin from left side
                                    */
    }

    /*Paired Margin*/
    div{
        margin: 10px 20px; /*10px margin from top and bottom side
                             20px margin from right and left side
                            */
    }


    Padding is same as margin! Replace "margin" keyword with "padding"
    
    -------------------------------------------------------------------
                TRBL (Top Right Bottom Left)
-------------------------------------------------------------------
-> Similar to margins
-> Useful while positioning elements in screen

-> Top
    -> amount of spacing from top of parent element
    Example: 

    div{
        top:<amount of spacing from top of parent element>
    }

-> Right
    -> Amount of Pixels from right of parent element
    Example: 

    div{
        top:<amount of spacing from right of parent element>
    }

-> Bottom
    -> amount of spacing from bottom of parent element
    Example: 

    div{
        top:<amount of spacing from bottom of parent element>
    }

-> Left
    -> Amount of Pixels from left of parent element
    Example: 

    div{
        top:<amount of spacing from left of parent element>
    }


-------------------------------------------------------------------
                            Positioning
-------------------------------------------------------------------

-> Determines how are objects positioned in browser window
-> 4 types

-> Static:
    -> Default Positioning
    -> TRBL donot work if an element is Staticaly Positioned
    Syntax: 
    position: static;

-> Relative
    -> Similar to static
    -> TRBL workd if an element is Relatively Positioned
    Syntax: 
    position: relative;

-> Absolute
    -> Usaully Applied to Child tags of any parent tag
    -> TBRL works
    -> Parent tag must have relative positioning
       else Body tag is treated as relative
       ELements are positioned relative to body tag
       Syntax
       position: absolute;

-> Fixed
    -> Elements are positioned relative to viewport
    -> Element is fixes to one place even while scrolling
    Syntax:
    position: fixed;

-> Sticky
    -> Combination of Fixed and Relative
    -> Element is fixed to viewport at specified TRBL position
    -> Any one among TRBL is compulsary to include
    Syntax:     
    position: sticky;

    Example:
        .static{
            position: static;
        }

        .relative{
            position: relative;
        }

        .relative .absolute-inside-relative-class{
            position: absolute;
        }
        .fixed{
            position: fixed;
        }
        .sticky{
            position:sticky;
        }

-----------------------------------------
            Link Tag
-----------------------------------------
-> A link tag must be selected on its own
    Either as Class name, ID name or Tag name
    The CSS properties are same.

-----------------------------------------
                Image 
-----------------------------------------
    - Height ant Width

        HTML:
        <img src="path">
        
        CSS:
        img{
            height: value;
            width: value;
        }
    
    object - fit
        -> Fit Image Relative to Screen
        img{
            object-fit: value;
        }


