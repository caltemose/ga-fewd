<div class="block"></div>

# FEWD - HTML BASICS

Chad Altemose<br>
<small>Sr Web Engineer @ Huge Inc.</small>

---

# Objectives

- Use Sublime Text to create and edit web files
- Use Google Chrome to view and debug web files
- Format text into semantic and valid HTML
- Link an external stylesheet to style HTML files


Note:
Objectives will always be shown in class.
<br>
We'll learn to use our text editor and other tools as well as how to test and debug in the browser.
<br>
We'll make some basic web pages.
<br>
Our homework for this week will be discussed at the end of lesson 2.

---

# Agenda

- <span class="talk">TALK</span> HTML Intro/Overview
- <span class="code">CODE</span> Mark up a press release
- <span class="talk">TALK</span> CSS Intro/Overview
- <span class="code">CODE</span> Style a press release
- <span class="lab">LAB</span> Markup and Style a Cookie Recipe

Note:
Define talk/code/lab/group symbols.<br><br>
Today we'll have brief lectures on intro material<br>
followed by code alongs<br>
then we'll finish with some lab time.

---

# Intro to HTML

- Basic page structure
- Semantics
- Core tags and example usage
- From HTML to HTML5

Note:
20-minute lecture || This is the outline.<br>
<br>
Semantics = meaning. We markup our content with HTML that defines our content's meaning, e.g., this content is a headline or this content is a paragraph.<br>
<br>
Brief discussion of the history of HTML.

----

## The Basics

- HTML: What it is
- CSS: What it looks like
- Javascript: What it does

Note:
Or to put it a different way:<br>

- semantics
- style
- functionality

----

## HTML Structure

```
<body>
   <h1>My Resume Page</h1>

   <section>
      <h2>About Me</h2>
      <p>First paragraph of my story.</p>
   </section>

```

Note:

- HTML describes the structure of a page with tags
- Each tag has implied semantic meaning
- Sometimes its meaning is obvious; sometimes it isn't
- Indentation is used to clarify parent/child structure


----

## Paired Tags

<pre class="large">
  <code>
   <h2>About Me</h2>
  </code>
</pre>


Note:
Most tags come in pairs and surround the content they are defining.
<br><br>
Opening and closing tags are identical except for the slash in the closing tag.

----

## Self-Closing Tags


```
<br/>   <hr/>   <input/>
```


Note:
- Some tags are used without a paired closing tag
- They'll become pretty obvious as your knowledge grows.
- The self-closing slash is no longer required.

----

## Headers

```
<h1>Primary Headline</h1>

<h2>Secondary headline</h2>

<h3>Tertiary headline</h3>
```

Note:
- Headers are some of the first tags we'll be using to classify headlines
- The numbers indicate the level/priority of that headline, 1 indicating the highest level and 6 indicating the lowest.

----

## Paragraphs

```
<p>Here is a short paragraph. It contains two sentences.</p>
```

----

## Attributes

```
<a href="/about">About Page</a>

```

Note:
- The anchor tag (```a```) is for linking to a place.
- Note the HREF attribute for adding information to a tag instance.
- Attributes let us custom configure tags and pass along custom data to the browser.

----

## Lists

```
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>Javascript</li>
</ul>
```

Note:
- Lists are very common.
- Start to think of them abstractly (navigation list, product items, comments).

----

## Images

```
<img src="photo.jpg" alt="Photo of Me">
```

Note:
The image tag lets us place images in the page.

- Attributes are critical in this tag.
- Shown are the minimum required attributes.
- Width and Height are missing but we will use those attributes whenever we can


----

## Forms

```
<form>
  <input type="text" name="first_name">
  <select name="gender">
    <option value="f">Female</option>
    <option value="m">Male</option>
  </select>
  <input type="submit" value="Submit!">
```

Note:
Remember we're not trying to memorize tags just yet; We're just starting to get familiar with them.
<br><br>
- Forms use tags for common interactive components, not just content.
- Attributes become more complex and necessary.
- We'll have an entire lesson in the future devoted to creating forms.

----

## From HTML to HTML5

updated HTML language specs with new tags and attributes

<br>

```
<section>
<aside>
<nav>
<header>
<input type="email">
```

Note:
- HTML5 the language = HTML + new tags/standards
- HTML5 the logo/buzzword = HTML5 + CSS3 + Javascript.
<br><br>
- This is a sample of new tags - not an exhaustive list.
- These tags give us more of a vocabulary to impart content with meaning/semantics.
- Any questions before we start coding?
- At the end of the slides we'll have a link to an exhaustive HTML5 tag list.

---

# Write Some HTML

### Press Release Semantics and Structure

- DOCTYPE
- Required boilerplate: head + body
- Semantics of the provided text
- Implementation
- [press release text](../../../Week_01_Basics/01_html_basics/starter_code/ga_press_release/release.txt)

Note:
- 50 minutes
- DOCTYPE defines what kind of document this is
- HEAD contains meta information: page title, links to CSS and JS, document description, etc)
- BODY contains all content/user interface
- Discuss semantics of press release (headline, date, body copy, footer)
- hipchat: https://ga-atl-fewd.hipchat.com/invite/171141/a2acfbc061c65b547d4628682299dcf4


---

# CSS Basics

### Brief Introduction

- Tags and Properties (basic structure)
- Cascading effect
- From CSS to CSS3
- Inline vs In-page vs External implementations

Note:
- 10 minutes
- CSS gives the web its style.
- We -suggest- styling to the browser via CSS. Browsers interpret as they see fit.

----

## CSS Basics
### Tags and properties

```
p {
  margin: 20px;
  color: blue;
}
```

Note:
- CSS uses selectors to determine what page elements you are styling. ```p```
- CSS styles properties of those selectors using values. ```margin: 20px```
- As we go through our lessons and code alongs, we'll expand our vocabulary of allowed properties and values.
- Properties are used for: structure/layout, type, interaction fx, animation

----

## CSS Basics
### From CSS to CSS3


```
p {
  border-radius: 4px;
  opacity: 0.5;
  transition: width 0.5s linear 1s;
}
```

Note:
- CSS3 is the modern version of CSS.
- CSS3 is not fully supported by all browsers.
<br><br>
Most newly-added properties add more complex behaviors than we have needed in the past like animation and mathematical transformations of content.
<br><br>
We'll become familiar with which CSS properties are safe to use and which properties are not yet fully supported.

----

## CSS Basics
### Implementation - External File

In a separate file ```styles.css```:

<br>

```
p {
  color: blue;
}
```


Note:
This is how we will write our styles 99% of the time. It is favored because of ease-of-development and sharing styles across pages for efficiency's sake.


----

## CSS Basics
### C is for Cascading

- parent > child relationships
- specificity
- priority

Note:
These are some basic concepts to pay attention to as we move through the course.
<br><br>
We'll be discussing these abstract concepts with examples throughout the course.

---

# Write Some CSS
### Styling the Press Release

- Implementing an external stylesheet
- Styling the headline
- Styling the body
- Observing the cascading effect

Note:
50 minutes

---

# Cookie Recipe

- 50-minute Lab
- [starter text](../../../Week_01_Basics/01_html_basics/starter_code/cookie_recipe/index.txt)
- [image](../../../Week_01_Basics/01_html_basics/starter_code/cookie_recipe/cookies.jpg)

Note:
50 minutes

---

# Final Thoughts

Study the basics. View source. <br>
Get familiar with the available tags and their usage.

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

