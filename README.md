# Responsive websites
Repo used for completing the "Build Responsive Real World Websites with HTML5 and CSS3" Udemy course.

Start date: Tuesday 22/1/2019

Finish date:

# Stuff learnt so far

## Section 2 - Intro to HTML

* 1 - Use '\<br>' as '\n' in java.

* 2 - Use 'alt' attribute inside an "img" tag to describe the image in case the browser can't display it. 

* 3 - Use an "a" tag with a 'href' attribute to create links. Links can be externals (to another websites or content outside our project) or internals (to images or content inside our project):
  * e.g:
    *  \<a href=http://www.facebook.com>Link to facebook\<a>.
    * \<a href=logo.jpg>Link to logo image\<a>.

* 4 - Use 'target' attribute inside an "a" tag to define wheter the link should be opened. For the same tab use <em>_self</em> for a new tab use <em>_blank</em>.
  * e.g:
    * \<a href=logo.jpg target="_self">Link to logo image\<a>.
    * \<a href=logo.jpg target="_blank">Link to logo image\<a>.


## Section 3 - Intro to CSS

* 1 - Use "link" tag to link CSSs files to the HTML. It must be placed in the HTML "header".<br>
  * e.g: \<link rel="stylesheet" type="text/css" href="style.css">

* 2 - CSS is rule based. Each rule has a selector (h1, h2, p, etc.) block and a decorator block (color, font-size, font-family, etc.).
  * e.g: 
    * h1{ <br> 
        color : green;<br>
        font-size: 30px;<br>
        font-family: Arial;
        }
    * p{<br> 
        color: crimson;<br>
        font-size: 15px;<br>     font-family: Arial;<br>
        }

* 3 - Common decorations can be combined in a single rule to prevent code repetition.
  * e.g: 
    * h1, p{<br>
            font-family: Arial;<br>
            }
    * h1{ <br> 
        color : green;<br>
        font-size: 30px;<br>
        }
    * p{<br> 
        color: crimson;<br>
        font-size: 15px;<br>
        }

* 4 - We can define a basic rule that applies to the whole body of the HTML (its visible part) and then override it with specific rules.
  * e.g: 
    * body{<br> 
        color: red;<br>
        font-family: Arial;<br>
        }
    * h1{ <br> 
        color : green;<br>
        font-size: 30px;<br>
        }
    * p{<br> 
        color: crimson;<br>
        font-size: 15px;<br>
        }

* 5 - Colors in CSS are formed by the combination of red, green and blue. Abbreviated as RGB, they're notated with two hexadecimal numbers for each color (#RRGGBB) obtaining up to 16M of colors from all the possible combinations.
  * e.g: 
    * #FF0000 => represents red color.
    * #00FF00 => represents green color.
    * #0000FF => represents blue.

* 6 - CSS colors can have transparency.  In order to use it, the notation has to be different from RGB. Each color HEX value is converted to decimal and then and an additional fractional number is used to define the grade of transparency.<br>
  * e.g: 
    * #00FF00 => rgba(0, 128, 0, 1.0).
    * #FF0000 => rgba(128, 0, 0, 0.75).

* 7 - HTML allows the definition of <strong>class</strong>es and <strong>id</strong>'s through the attributes 'class' and 'id'. This attributes can be applied to <em> any </em> tag of the HTML file but id's must be unique inside each HTML file and can be applied to one tag only.
  * e.g: 
    * \<body class='main-text> <em>...paragraph text goes here...</em>\</body>.
    * \<h1 class='header-text> <em>...header 1 text goes here...</em>\</h1>.
    * \<p id='author-text'><em>...author text goes here...</em>\</p>

* 8 - The usage of classes and id allows CSS to apply the same decoration to all the elements falling under the same class/id attribute. Use '.' (dot) before specifying the class name and '#' (hashtag) before the id.
  * e.g: 
    * .main-text{<br> 
        text-align: right<br>
        }
    *   .random-text{<br> 
        text-align: center;<br>
        }
    * .author-text{<br> 
        font-size: 22px;<br>
        }

* 9 - The usage of id's is <strong>not a good practice</strong> because they can't be reused! Use classes instead!

* 10 - CSS box model says that every HTML element can be seen as a box. This allows the definition of the space between elements among other things. <br><br> 
![Sarah](css_box_model.png)


  



