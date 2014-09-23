<div class="block"></div>

# FEWD - CSS BASICS

Chad Altemose<br>
<small>Sr Web Engineer @ Huge Inc.</small>

---

# Objectives

- Explain CSS cascading effect
- Apply CSS to take advantage of cascading
- Define the DOM
- Apply relative and absolute paths to images and links
- Experiment with margin and border

---

# Agenda

- <span class="talk">talk</span> Review HTML Images and Paths
- <span class="group">group</span> Plan markup for Wendy Bite page
- <span class="code">code</span> Use ```<img>``` to add images to a page
- <span class="talk">talk</span> Review CSS Colors
- <span class="code">code</span> Begin Styling Wendy Bite page
- <span class="lab">lab</span> Add Wendy G. Bite Resume page

---

# HTML Review

Note:
a little review, some new tags.

----

## More Structural Tags

```
 <div>
 <span>
```

Note:
unsemantic tags, use when there's no good alternate.
.
block vs inline, css box model coming soon.

----

## More Content Tags

```
<small>
<strong>
<code>
<cite>
<sup>
```

Note:
Tags that wrap chunks of content to add meaning.
.
Questions before new material?

----

## File Paths

Images are placed using the ```<img>``` tag:

```
<img src="img/image-name.jpg" alt="description of this image.">
```

Note:
The img tag requires a src attribute which tells the browser where to find the image.
.
This path is relative starting at the HTML file, going into 'img'

----

## File Paths

![a](../../img/lessons/directory-tree.jpg)


Note:
- relative: class preference
- full: requires server (notice file:///)
- absolute: best left for files on different servers (cdn, etc)
- ../  /  http[s]://  file:///

----

## Image alt attributes

    <img src="puppy.jpg" alt="My cute puppy">

Note:
When text is shown depends on browser: loading, missing image, images unloaded (eg email)
.
More linguistic context (seo) about the image as it is used on your page.
.
Reasons an image may not load: connection error, file not found, lynx/etc, screen reader reads alt text

----

## Image Formats

There are three main image file formats:

- jpg
- png
- gif

Note:
List sorted by likelihood of use.
.
Some basic rules:
photo -> jpeg
transparency -> png24
truly limited colors -> png8
rudimentary animation -> gif

----

## Image: JPEG

![a](../../img/lessons/green-sticks.jpg)

Note:
No transparency, can be stored at different compression levels with varying amounts of "lossy-ness", typically the best format for photos. (Try to balance between photo quality and file size.)

----

## Image: PNG

![a](../../img/lessons/ga-logo-transparent.png)

Note:
Supports transparency and semi-transparency, great for logos, icons, and repeating background tiles.
.
Almost always preferable to a gif.


----

## Image: GIF

![a](../../img/lessons/ram-rider.gif)

Note:
Can have basic transparency, typically a `png` is used instead.

---

# About Me Markup

- [Preview image](../../../Week_01_Basics/02_css_basics/starter_code/WendyBite_AboutMe_final.png)
- Plan markup/structure
- Create initial files, boilerplate
- Add [content](../../../Week_01_Basics/02_css_basics/starter_code/Wendy_Bite.txt)

Note:

---

## CSS Colors: Keywords


Simplest but used infrequently:

    color: white;

<br>

<small>See [here](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value#Color_keywords) for a list of colors and sample swatches.</small>

Note:
Colors ultimately specified as RGB colors whether keyword, hex or rgb/a.

----

## CSS Colors: Hex Codes

![Hex Color explanation](../../../img/lessons/web-colors.svg)

Note:
Explain RGB/color-as-light (additive) vs color-as-ink (subtractive)<br>
Math/theory not important unless you're gonna be a dev and then it's pretty easy to learn the patterns.
.
Doubling (#6f0)

----

## CSS Colors:  RGB

```
color: rgb(255, 0, 0);
```

Note:
Starting to be preferred method.
.
A little easier to read.
.
RGBA.

---

# About Me Styles

- basic content styling
- aligning images
- apply border and padding to image
- review and apply common ```hr``` styling
- review and use a ```div``` wrapper container
- [Preview image](../../../Week_01_Basics/02_css_basics/starter_code/WendyBite_AboutMe_final.png)

Note:

---

# Create and Link the Resume Page

- link ```<a>``` navigation tags to pages
- discuss path relationships in terms of linking
- duplicate the landing page as a template

Note:
use anchors to link to other pages.
.
paths not just for images.
.
you handle the duplicating and remainder of work.


---

# Final Thoughts

Study the basics. View source. <br>
Get familiar with the available tags and their usage.<br>
Get familiar with style properties and expected values.

<br>

- [HTML tag reference](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5/HTML5_element_list)
- [CSS property reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)
- [Chris Coyier CSS Site](http://css-tricks.com/)
- [HTML & CSS Book](http://htmlandcssbook.com/)

Note:
Use developer tools. View source. Memorize tags.


---


# Homework

- Create a [resume website](../../../Week_01_Basics/01_html_basics/Assignment/index.html)
- [Watch a video on the Internet about the Internet](https://www.youtube.com/watch?v=7_LPdttKXPc)
