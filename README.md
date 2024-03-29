<!DOCTYPE html>

<html lang="en">

<head>
    <title>CSS Part 2</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles/main.css">

    <link rel="stylesheet" href="styles/csspart2.css">
    <link rel="stylesheet" href="https://code.jquery.com/qunit/qunit-2.9.2.css">
    <link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
</head>

<body>
    <header>
        <nav id="navMain">
            <a href="index.html">Home</a> |
            <a href="wwwintro.html">WWW Intro</a> |
            <a href="htmlstructure.html">HTML Structure</a> |
            <a href="htmlcontent.html">HTML Content</a> |
            <a href="dataimport.html">Data Import Formats</a> |
            <a href="csspart1.html">CSS Part 1</a> |
            <a href="csspart2.html">CSS Part 2</a> |
            <a href="design.html">Design Issues</a>
        </nav>

    </header>
    <div id="divContent">
        <section id="sectionMain">
            <h1>CSS Part 2</h1>

            <section id="practicearea" >
                <h2>Practice Area</h2>
                <!--Further Work -->
                <div id="divAnimate"></div>
            </section>

            <section id="studentcode">
                <style>
                    #secStatic{
                        Position:Static;
                        color: rgb(30, 0, 200);
                        Border:3px solid;
                        border-color:rgb(0, 110, 255);
                        Background-color:rgb(139, 212, 246);
                        Width:300px;

                    }

                    #secRelative{

                        Position:Relative;
                        Left:100px;
                        Color:rgb(12, 68, 2);
                        Border:3px solid;
                        border-color: rgb(115, 173, 33);
                        Background:rgb(173, 246, 139);
                        width:300px;
                    }

                    #secFixed{
                        Position:Fixed;
                        Bottom:300px;
                        Right:180px;
                        Color:rgb(45, 2, 49);
                        Border:3px solid;
                        border-color:rgb(173, 33, 126);
                        Background-color:rgb(246, 139, 237);
                        Width:300px;

                    }

                    #secAbsolute{
                        Position:Absolute;
                        Top:240px;
                        Left:330px;
                        Color:rgb(38, 39, 1);
                        Border:3px solid;
                        border-color:rgb(173, 140, 33);
                        Background:rgb(230, 248, 128);
                        Width:300px;


                    }

                    #divFloatLeft{
                        Float:Left;
                        Border:3px solid;
                        border-color:rgb(117, 33, 173);
                        Background:rgb(214, 188, 221);

                    }
                    
                    #divFloatRight{
                        Float:Right;
                        Border:3px solid;
                        border-color:rgb(117, 33, 173);
                        Background:	rgb(214, 188, 221);

                    }

                   #divRotate{
                       Position:Relative;
                       Top:130px;
                       Transform: rotate(20deg);
                       Border:3px solid rgb(173, 33, 75);
                       Background:rgb(221, 188, 198);
                       Width:300px;
                   }

                   

                </style>

                <h2>Student Code Area</h2>
                <section id="secPositioning">
                    <section id="secStatic" class="testSection">
                        <h3>Static positioning</h3>
                        <p>HTML elements are positioned static by default. Static positioned elements are not affected by the top, bottom, left, and right properties. An element with position: static; is not positioned in any special way; it is always positioned according to the normal flow of the page</p>
                    </section>
                    <section id="secRelative" class="testSection">
                        <h3>Relative positioning</h3>
                        <p>An element with <code>position: relative;</code> is positioned relative to its normal position. Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position. Other content will not be adjusted to fit into any gap left by the element.</p>
                    </section>
                    <section id="secFixed" class="testSection">
                        <h3>Fixed positioning</h3>
                        <p>An element with <code>position: fixed;</code> is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element. A fixed element does not leave a gap in the page where it would normally have been located.</p>
                    </section>
                    <section id="secAbsolute" class="testSection">
                        <h3>Absolute positioning</h3>
                        <p>An element with <code>position: absolute;</code> is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed). Jf an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.</p>
                    </section>
                    <section id="secFloat">
                        <div id="divFloatLeft" class="testSection">
                            <h3>Float Left</h3>
                        </div>
                        <div id="divFloatRight" class="testSection">
                            <h3>Float Right</h3>
                        </div>
                    </section>
                    <section id="secTransform">
                        <div id="divRotate">
                            <h3>Rotate</h3>
                        </div>
                    </section>
                    <!-- W3.CSS Section - styles applied in class attributes -->
                    <section id="secW3CSS">
                        <div id="divW3CSS" class="w3-container w3-teal">
                            <h3>W3.CSS</h3>
                            <p>W3.CSS is a modern CSS framework with built-in responsiveness. It supports responsive mobile first design by default, and it is smaller and faster than similar CSS frameworks. W3.CSS can also speed up and simplify web development because it is easier to learn, and easier to use than other CSS frameworks:</p>
                            <p>Note that the styles for this W3 container must be correct for the following W3 Card tests to pass.</p>
                        </div>
                        <div id="divCard" class="w3-card-4 w3-margin w3-light-gray ">
                           <img id="imgCard" src="images/house.jpg" alt="House">
                                 <div id="divSubCard" class="w3-container w3-center">
                                    <p>Recent newbuild - one careful owner</p>
                                    <p>Note that the styles for this card will not pass the tests until the previous W3 container styles have been correctly set.</p>
                                </div>
                        </div>
                        <div id="divW3Row" class="w3-row">
                            <div id="divW3Col1" class="w3-col m4 l3 w3-container w3-blue ">
                                <p>This part will occupy 12 columns on a small screen, 4 on a medium screen, and 3 on a large screen.</p>
                            </div>
                            <div id="divW3Col2" class="w3-col m8 l9 w3-container w3-amber ">
                                <p>This part will occupy 12 columns on a small screen, 8 on a medium screen, and 9 on a large screen.</p>
                                <p>This part will occupy 12 columns on a small screen, 8 on a medium screen, and 9 on a large screen.</p>
                            </div>
                        </div>
                    </section>
                </section>

            </section>    
        </section>
        <aside id="asideMain">
            <div id="divAsideHeight">
                <h2>Tips/Links</h2>
                <q class="tip">Don't forget to backup you work on a regular basis.</q>
                <q class="tip">Don't forget to use the Browser Developer Tools to help debug your code.</q>
                <q class="tip">Don't forget to make sure your code is <a href="https://validator.w3.org/" target="_blank">validated</a></q>
                <p><a href="https://www.w3schools.com/html/html5_syntax.asp" target="blank">W3Schools Coding Conventions</a></p>
                <p><a href="https://loremipsum.io/generator/?n=2&t=p" target="_blank">Lorem ipsum Generator</a></p>
                <p><a href="https://validator.w3.org/#validate_by_input" target="_blank">W3C Validator</a></p>
            </div>
        </aside>
    </div>

    <footer id="footerMain">
        <nav id="navFooter">
            <a href="index.html">Home</a> |
            <a href="wwwintro.html">WWW Intro</a> |
            <a href="htmlstructure.html">HTML Structure</a> |
            <a href="htmlcontent.html">HTML Content</a> |
            <a href="dataimport.html">Data Import Formats</a> |
            <a href="csspart1.html">CSS Part 1</a> |
            <a href="csspart2.html">CSS Part 2</a> |
            <a href="design.html">Design Issues</a>
        </nav>
    </footer>
    <div id="qunit"></div>
    <div id="qunit-fixture"></div>
    <script src="https://code.jquery.com/qunit/qunit-2.9.2.js"></script>
    <script src="scripts/testCSS2.js"></script>
</body>

</html>
