# Class-05

## Images

The HTML `<img>` tag is used to embed an image in a web page. It is an empty tag (does not have a closing tag).

The <img> tag has two required attributes:

- src - Specifies the path to the image
- alt - Specifies an alternate text for the image

*Syntax:*
`<img src="url" alt="alternatetext">`

### Three Rules for Creating Images:

1. Save images in the right format: Websites mainly use images in *jpeg, gif, or png*.

2. Save images at the right size: You should save the image at the same width and height it will appear on the website.

3. Use the correct resolution Computer screens are made up of dots known as *pixels*. Images created for the web should be saved at a resolution of 72 ppi. The higher the resolution of the image, the larger the size of the file.

- Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.

----

 ## Color

![css](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT0UvTY_q11Imi02CXns6P54eFo_YwzJIEGLg&usqp=CAU)

The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:

1.	**rgb values**
These express colors in terms
of how much red, green and blue are used to make it up. For example: `rgb(100,100,90)`

![](https://tutorial.techaltum.com/images/css-colors.jpg)


1.	**hex codes**
These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: `#ee3e80`

![](data:image/png;base64,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)

1.	**color names**
There are 147 predefined color names that are recognized by browsers. For example: `DarkCyan`.

![](https://cdn.educba.com/academy/wp-content/uploads/2020/03/CSS-Color-Codes.jpg)


| Hue     | is the colloquial idea of color    | 
| Saturation | is the amount of gray in a color   | 
| Lightness  | is the amount of white (lightness) or black (darkness) in a color | 
| Values   | Put Pipes In | 




The **hsl** color property has been introduced in *CSS3* as an alternative way to specify colors. The value of the property starts with the letters hsl, followed by individual values inside parentheses for:

- *hue* : This is expressed as an angle (between 0 and 360 degrees).
- *saturation* : This is expressed as a percentage.
- *lightness* : This is expressed as a percentage with 0% being white, 50% being normal, and 100% being black.

CSS3 allows you to specify colors as hsl values, with an optional opacity value. It is known as `hsla`, while tha a is for alpha.

- alpha: fourth value which represents transparency This is expressed as a number between 0 and 1.0  .


![](https://i0.wp.com/www.cssscript.com/wp-content/uploads/2017/01/Minimal-HSLA-Color-picker-With-Pure-JavaScript.png?fit=543%2C408&ssl=1)


CSS3 Also, has introduced an extra value for `rgb` colors to indicate opacity. It is known as `rgba`. 

----

## Text

- There are properties to control the choice of font, size, weight, style, and spacing.

  *Example:*
   `font-style: italic;`  
   `font-weight: bold;`

- There is a limited choice of fonts that you can assume most people will have installed because that a browser will usually only display it if it's installed on that user's computer.

- If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.

- You can control the space between lines of text (`line-height: 1.4em;`), individual letters (`letter-spacing: 0.2em;`), and words (`word-spacing: 1em;`). 

- Text can also be **aligned** to the left, right, center, or justified (This indicates that every line in a paragraph,except the last line, should be set to take up the full width of the containing box.). It can also be **indented**.

  *Example:*
   `text-align: left;`
   `text-indent: 20px;`

- You can use pseudo-classes to change the style of an element when a user hovers `:hover` over or clicks on text, or when they have visited `:visited` a link.


![](https://i1.wp.com/www.tutorialbrain.com/wp-content/uploads/2019/03/CSS-Font-Property_tutorialbrain.png?fit=800%2C800&ssl=1)
