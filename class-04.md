## Links

Links allow users to click their way from page to page. They are created by using the <a> element and the href attribute to indicate the page you are linking to, like below:

![](https://learn-the-web.algonquindesign.ca/topics/html-semantics/html-tag-parts.png)

### Absolute and Relative URLs:

- Absolute URL: a full web address.

- Relative URL: A local link (a link to a page within the same website) _without the "https://www" part_.

  - If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.

- You can create links to open email programs with an email address. The href attribute starts with `mailto:` and is followed by the email address you want the
  email to be sent to.

_Example:_
`<a href="mailto:email@example.jo">`

### Target:

If you want a link to open in a new window, you can use the target attribute on the opening `<a>` tag. The value of this attribute should be `_blank`.

_Example:_
`<a href="http://www.imdb.com" target="_blank">`

- You can use the id attribute to target elements within a page that can be linked to.

_Example:_
`<p><a href="#top">Top</a></p>`

-----

## Layout

**Block-level** boxes start on a new line and act as the main building blocks of any layout(such as `<h1>` `<li>` ), while **Inline** boxes flow between surrounding text (such as `<img>` ).

### Containing Elements:

The containing or _parent_ element is the outer box which contain a block-level element sits inside another block-level element. It is common to group a number of elements together inside a <div> (or other block-level) element.

### Controlling the Position

CSS has allow you to control the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.

1. **Normal flow**: Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. This is the default behavior.

2. **Relative Positioning**: This moves an element from the position it would be in normal flow. This
   does not affect the position of surrounding elements.

3. **Absolute positioning**: This positions the element in relation to its containing element. It is taken out of normal flow.Absolutely positioned elements move as users scroll up and down the page.

- To indicate where a box should be positioned, you may also need to use **box offset** properties to tell the browser how far from the top or bottom and left or right it should be placed.
----

## Function

A JavaScript function is a block of code designed to perform a particular task and it is executed when calls it(_invokes_).

![](https://s3.ap-south-1.amazonaws.com/s3.studytonight.com/tutorials/uploads/pictures/1587882057-1.png)

- You can invokes the function by use the function name followed by parentheses.
- If the function have _parameters_ when it is invoked it should have _arguments_ (the values received by the function).
- When JavaScript reaches a return statement, the function will stop executing.
-----

## 6 Reasons for Pair Programming


**How does pair programming work?**

*While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted into code while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code*

1. Greater efficiency

2. Engaged collaboration

3. Learning from fellow students

4. Social skills

5. Job interview readiness

6. Work environment readiness

to know more about this [click here](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)