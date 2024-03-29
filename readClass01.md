# Responsive Web Design

Is building a website to work on every device and every screen size, mobile or desktop,providing an intuitive and gratifying experience for everyone.

Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation.

### Responsive web design components:

- flexible layouts: capable of dynamically resizing to any width.
- media queries: provide the ability to specify different styles for individual browser.
- flexible media: media types need to be scalable (changing their size as the size of the viewport changes).

_There are two ways to use media queries:_

- the @media rule inside of an existing style sheet.
- linking to a separate style sheet from within the HTML document.

![](https://www.csssolid.com/images/css-media-query.png)

## Float

Float is CSS positioning property when set the images into the page that text wraps around them as needed.or Ignoring the text wrap will allow the words to flow right over the image like it wasn’t even there.

And when use absolute positioning to page element will not affect the position of other elements and other elements will not affect them.

![](https://images.slideplayer.com/34/8403951/slides/slide_114.jpg)

Clear has four valid values as well. **Both** is most commonly used, which clears floats coming from either direction. **Left** and **Right** can be used to only clear the float from one direction respectively. clearing the float will move itself down past the float.

![](https://css-tricks.com/wp-content/uploads/2020/12/unclearedfooter.png)

### Problems with Floats

- Pushdown: Most browsers will render the image outside the float, but not have the part sticking out affect other layout. To fix it use `overflow: hidden` to cut off excess.

- Double Margin Bug: if you apply a margin in the same direction as the float, it will double the margin. To fix it set `display: inline` on the float.

## SMACSS

- SMACSS (Scalable and Modular Architecture for CSS): is a way to examine your design process and as a way to fit those rigid frameworks into a flexible thought process.

![](https://habrastorage.org/files/4dc/24a/8dc/4dc24a8dc3fb4e758adf89af4f73f66c.png)
