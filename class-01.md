# Ducket HTML book
# Introduction
* Firstly,the book has been written with two very different types of people in mind:
  1. Those who want to learn how to design and build websites from scratch.
  2. Anyone who has a website and wants more control over the appearance of their pages.
* Many books that teach HTML and CSS resemble dull manuals. To make it easier for you to learn, we threw away the traditional
  template used by publishers and redesigned this book from scratch.
* In order to teach you about creating web pages, this book is divided into three sections:
  1. HTML:We will spend the first chapter looking at how HTML is used to create web pages.
  2. CSS: We start this section with a chapter that explains how CSS uses rules to enable you to control the styling and layout of web pages.
  3. practical: We end up with some helpful information that will assist you in building better websites.
 * Before we look at the code used to build websites it is important to consider the different ways in which people access the web and clarify some terminology.
  1. **Browsers :** People access websites using software called a web browser. Popular examples include Firefox, Internet Explorer, Safari, Chrome, and Opera.
  2. **Web Servers :** When you ask your browser for a web page, the request is sent across the Internet to a special computer known as a web server which hosts the website.
 * **How Websites Are Created** :All websites use HTML and CSS, but content management systems, blogging software, and e-commerce platforms often add a few more technologies into     the mix.
 * **How the Web Works**: When you visit a website, the web server hosting that site could be anywhere in the world. In order for you to find the location of the web server, your     browser will first connect to a Domain Name System (DNS) server.
  # chapter1: Structure
  * **HTML Describes the Structure of Pages**
  * **HTML Uses Elements to Describe the Structure of Pages**
     * Each element has an opening tag and a closing tag,`<h1>This is the Main Heading</h1>`.
     * Tags act like containers. They tell you something about the information that lies between their opening and closing tags,`<p lang="en-us">Paragraph in English</p>`.
   # Chapter 8:Extra Markup
   * **The Evolution of HTML**: Since the web was first created, there have been several different versions of HTML.
     * **DOCTYPEs**:each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using, example HTML5 `<!DOCTYPE html>`.
   * **Add comments in HTML using** `<!-- comment goes here -->`
   * **ID Attribute** :Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page.example `<p id="pullquot"      </p>`.
   * **Class Attribute**:Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one element within a document, you will want away to          identify several elements as being different from the other elements on the page.example `<p class="important"></p>`.
   * **Block Elements**: Some elements will always appear to start on a new line in the browser window. These are known as block level elements.Examples of block elements are
     `<h1>, <p>, <ul>, and <li>.`
   * **Inline Elements**:Some elements will always appear to continue on the same line as their neighbouring elements. These are known as inline elements.
       Examples of inline elements are `<a>, <b>, <em>, and <img>.`
   * The `<div>` and `<span>` elements allow you to group block-level and inline elements together.
   * `<iframes> `cut windows into your web pages through which other pages can be displayed.
   * The `<meta>` tag allows you to supply all kinds of information about your web page.
   * Escape characters are used to include special characters in your pages such as `<, >, and ©.`
  
  
