# Responsive websites
Repo used for completing the "Build Responsive Real World Websites with HTML5 and CSS3" Udemy course.

Start date: Tuesday 22/1/2019

Finish date:

# Stuff learnt so far

## Section 2 - Intro to HTML

* 1 - Use '\<br>' as '\n' in java.

* 2 - Use 'alt' attribute inside an "img" tag to describe the image in case the browser can't display it. 

* 3 - Use an "a" tag with a 'href' attribute to create links. <br> 
    * Links can be externals (to another websites or content outside our project):<br>
e.g: \<a href=http://www.facebook.com>Link to facebook\<a>.<br>
    * Links can be internals (to images or content inside our project):<br>
e.g: \<a href=logo.jpg>Link to logo image\<a>.

* 4 - Use 'target' attribute inside an "a" tag to define wheter the link should be opened.
    * In the same tab (_self):<br>
    e.g:\<a href=logo.jpg target="_self">Link to logo image\<a>.
    
    * In a new tab (_blank):<br>
    e.g:\<a href=logo.jpg target="_blank">Link to logo image\<a>.


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

  



