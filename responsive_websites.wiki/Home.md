Welcome to the responsive_websites wiki!

## Section 2 - Dive into HTML

* 1 - Use '\<br>' as '\n' in java.

* 2 - Use 'alt' attribute inside an "img" tag to describe the image in case the browser can't display it. 

* 3 - Use an "a" tag with a 'href' attribute to create links. Links can be externals (to another websites or content outside our project) or internals (to images or content inside our project):
  * e.g:
    *  \<a href=http://www.facebook.com>Link to facebook\<a>.
    * \<a href=logo.jpg>Link to logo image\<a>.

* 4 - Use 'target' attribute inside an "a" tag to define wheter the link should be opened. For the same tab use <em>_self</em> and for a new tab use <em>_blank</em>.
  * e.g:
    * \<a href=logo.jpg target="_self">Link to logo image\<a>.
    * \<a href=logo.jpg target="_blank">Link to logo image\<a>.

* 5 - HTML allows the definition of <strong>class</strong>es and <strong>id</strong>'s through the attributes 'class' and 'id'. This attributes can be applied to <em> any </em> tag of the HTML file but id's must be unique inside each HTML file and can be applied to one tag only.
  * e.g: 
    * \<body class='main-text> <em>...paragraph text goes here...</em>\</body>.
    * \<h1 class='header-text> <em>...header 1 text goes here...</em>\</h1>.
    * \<p id='author-text'><em>...author text goes here...</em>\</p>

* 6 - The "div" element allows to divide the web into sections, creating pseudo-containers to store our content inside them. As with other elements, "div" tag can be decorated using CSS too.
  * e.g: 
    * \<div><br>
    \<h1><em>...h1 text goes here...</em>\</h1><br>
     \<h2><em>...h2 text goes here...</em>\</h1><br>
    \<p><em>...p text goes here...</em>\</p><br>
    \</div>

## Section 3 - Formatting with CSS

* 1 - Use "link" tag to link CSSs files to the HTML. It must be placed in the HTML "header".<br>
  * e.g: \<link rel="stylesheet" type="text/css" href="style.css">

* 2 - CSS is rule based. Each rule has a selector (h1, h2, p, etc.) and a decoration block (color, font-size, font-family, etc.).
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
        color: green;<br>
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

* 7 - The usage of HTML classes and id's allows CSS to apply the same decoration to all the elements falling under the same class/id attribute. Use '.' (dot) before specifying the class name and '#' (hashtag) before the id.
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

* 8 - The usage of id's is <strong>not a good practice</strong> because they can't be reused! Use classes instead!

* 9 - CSS box model says that every HTML element can be seen as a box. This allows the definition of the space between elements among other things. Everything, except the content of an element, is a CSS property and can be applied to the whole box or to a specific side (top, left, bottom or right).<br><br> 
![CSS box model](https://drupal.ed.team/sites/default/files/inline-images/box-model.png)
  *  Content: text, images, etc.  
  *  Padding: transparent area around the content and inside of a box.
  *  Border: wraps the padding and content. Can be transparent, or not.
  *  Margin: space between boxes.

* 10 - Default CSS box model has the <em>disadvantage</em> of only setting the height and width of the content instead of the entire box <em>(aka element)</em>. So padding, border and margin are values added to the height and width previously defined, which isn't a good idea.<br><strong>Solution:</strong> use the "box-sizing" CSS property and set it to 'border-box' to define the height and width of the whole box instead of the content only.

* 11 - To define the properties of an element (padding, border or margin), do it inside its own rule.
  * e.g:
    * h1{ <br> 
        font-size: 40px;<br>
        margin-bottom: 20px;<br>
        }
    * h2{ <br> 
        font-size: 30px;<br>
        margin-bottom: 10px;<br>
        }

* 12 - The "float" CSS property allows to put block elements side-by-side. It's a very interesting property because an element can be pushed left or right, allowing other elements to wrap around it.<br>To move other elements <strong>to the right of the selected one</strong>, set "float" to 'left' => the element will be floated to the left, causing all other elements to move to its right.<br>To move other elements <strong>to the left of the selected one</strong>, set "float" to 'right' => he element will be floated to the right, causing all other elements to move to its left.
  * e.g: 
    * .blog-post{ <br> 
        background-color: #0000FF;<br>
        width: 75%;<br>
        float: left;<br>
        }
    * .other-posts{ <br> 
    background-color: #00FF00;<br>
    width: 25%;<br>
    float: left;<br>
    }

* 13 - The cleanest way of defining the margins of a box is using the "margin" property which is allows to set all of them in the same line. The order is clock-wise (top, right, bottom, left).
  * e.g:
    * .container{ <br> 
        margin: 20px auto 0 auto;<br>
        }

* 14 - To define the borders of a box use the "border" property (border-top/right/bottom/left). Its input values are: width, type and color.
  * e.g:
    * .author-box{ <br> 
        border-top: 1px solid #808080;<br>
        }

* 15 - Use the 'img' CSS selector to format all the images inside of a box that has assigned a <strong>previously defined class</strong>.
  * e.g:
    * .author-box{ <br> 
        border-top: 1px solid #808080;<br>
        padding-top: 20px;<br>
        }
    * .author-box img{ <br> 
        height: 100px;<br>
        widht: 100px;<br>
        border-radius: 50%;<br>
        float: left;<br>
        margin-bottom: 20px;<br>
        }

* 16 - Elements with <strong>absolute positioning</strong> can be positioned <em>everywhere</em> we want inside their parent elements <strong>if and only if</strong> the parent positioning <em>is relative</em>.<br>
  * e.g: (blog-post is date's parent class)
    * .blog-post {<br>
        width: 75%;<br>
        float: left;<br>
        padding-right: 30px;<br>
        position: relative; <br>
    }
    * .date{<br>
        position: absolute;<br>
        top: 10px;<br>
        right: 30px;<br>
    }

## Section 4 - Web design basics

* 1 - Typography tips:
  * Use font size between 15px and 25px.
  * Use <strong>really big</strong> sizes for headlines, 32px +.
    * It may be a good idea to decrease font weight too.
  * Use linespaces (vertical spaces between lines) between 120-150%.
  * Each line should have 45 to 90 characters.
  * Make sure to choose the most adequate fonts based on the type of website.
    * Sans-serif family is one of the most used.
  
* 2 - Color tips:
  * Use a <strong>single</strong> base color for the web design.
  * <strong>Never</strong> use black for any part of the design.

* 3 - Color feelings:
  * <strong>Red</strong> transmits power, passion, strength and excitement.
    * Brighter tones are energetic.
    * Darker shades are more powerful and elegant.
  * <strong>Orange</strong> transmits cheerfullness and creativity.
    * Draws attention without being overpowered as red.
    * Can be associated with friendliness, confidence and courage.
  
  * <strong>Yellow</strong> transmits energy and gives the feeling of happiness and liveliness.
    * Can be associated with curiosity, intelligence and brightness.
  
  * <strong>Green</strong> transmits harmony, nature, life and health.
    * Can be associated with money.
    * In design causes a balancing effect and harmony effect.
  * <strong>Blue</strong> transmits patience, peace, trustworthiness and stability.
    * One of the most beloved colors, especially bye men.
    * Associated with professionalism, trust and honor.
  
  * <strong>Purple</strong> transmits power, nobility and wealth.
    * Can give a sense of wisdom, royalty, nobility, luxury and mistery.
  * <strong>Pink</strong> expresses romance, passivity, care, peace and affection.
  * <strong>Brown</strong> transmits relaxation and confidence.
    * Can be associated to earthiness, nature, durability, comfort and reliability.
  
  * For <strong>more information</strong> about colors take a look at "Color Theory" articles inside the <em>color</em> folder.

* Text over images tips:
  * Put text directly on the image <strong>if and only if</strong> it's quite dark and the text is white, otherwise <strong>don't do it</strong> because they won't contrast!
  
  * <strong>Overlay</strong> the image with <strong>a color</strong>, normally black, and then put the text on top of it.
  
  * <strong>Overlay</strong> the image with <strong>color gradients</strong> to achieve better results => use the color tips above to find the best color gradient.
  
  * Put the text <strong>in a box</strong>. The box should be opaque and transparent to achieve a better contrast.
  
  * <strong>Blur</strong> the image. It's very powerful and good looking. You can blur the whole image or use an out-of-focus area of a photo as the blur => Make sure the text stays at the <strong>same position</strong> on all screen resolutions.

  * <strong>Floor-fade</strong> the image. It's a technique where an image subtly fades towards black at the bottom with white text written over it. It's unnoticeable and improves readibility a lot!

## Section 5 - The killer website project





## Section 6 - Responsive web design with media queries




## Section 7 - Let's add some cool effects





## Section 8 - Optimizing and launching our website





    


  



