# 0x00. Advanced HTML

**HTML | Front-end**

**Concepts**

*For this project, we expect you to look at this concept:*

* [HTML - elements of a web page](https://intranet.alxswe.com/concepts/543)

## Welcome!

Welcome to the Web Stack specialization. The 3 first projects will give you all basics of the Web development: HTML, CSS and Developer tools.

In this project, you will learn how to use HTML tags to structure a web page. No CSS, no styling - don’t worry, the final page will be “ugly” it’s normal, it’s not the purpose of this project.

Important note: details are important! lowercase vs uppercase / wrong letter… be careful!

## Resources

**Read or watch:**

* [HTML 5.2](https://html.spec.whatwg.org/multipage/)
* [HTML: HyperText Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML)
* [HTML Reference - A free guide to all HTML elements and attributes](https://htmlreference.io/)
* [Can I use… Support tables for HTML5, CSS3, etc](https://caniuse.com/)
* [HTML Cheat Sheet - WebsiteSetup](https://websitesetup.org/html5-cheat-sheet/)

## Learning Objectives

At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

* Which guidelines to follow for HTML
* How to create the skeleton of an HTML5 page
* How to use semantic HTML tags to structure a web page
* Which use cases to use div vs span
* The semantic value’s of header, main, footer, article, nav, section, aside
* How to use headings (and why it’s important to follow the hierarchical order)
* How to make lists in HTML
* The differences between medias (SVG, GIF, PNG, JPG)
* How to structure data in a table
* How to integrate a video in a webpage
* How to integrate an audio file in a webpage
* How to embed external content
* How to correctly structure an HTML page

## Requirements

* A README.md file at the root of the folder of the project is mandatory
* Your code should be W3C compliant and validate with W3C-Validator
* Techium will be the name of the company we will use across our webpages.

## Sitemap of the project

![Site Map](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/4/4dec2ba9d84a0a55355b1c1e2de4c57854a2d35a.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231005%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231005T140651Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=4609f796a141613534ce593e0536adc6e657de333e35f9ab88772492ddeb6e50)

## Wireframe of Techium project
[Wire Frame](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/4/3e4f9e2b3cb73d1768229e086f5da35337be5c6c.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231005%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231005T140651Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=f4a4957470d9fbab7d583f47207943fc68d93125537d6d17c5f03afbd04daeec)

## Tasks

0. [Create your first webpage](./0-index.html)

Create your first HTML file 0-index.html with:

* Add the doctype on the first line (without any comment)
* After the doctype, open and close a html tag
* Add the language tag, specify English for ISO language code and add the direction tag (ltr or rtl) on the html tag.
* Open your file in your browser (the page should be blank)
W3C won’t pass - you can ignore it

**Repo:**

* GitHub repository: alx-frontend
* Directory: 0x00-html_advanced
* File: 0-index.html

1. [Structure your webpage](./1-index.html)

Copy the content of 0-index.html into 1-index.html

Create the head and body sections

* inside the html tag, create the head and body tags (empty) in this order

W3C won’t pass - you can ignore it

**Repo:**

* GitHub repository: alx-frontend
* Directory: 0x00-html_advanced
* File: 1-index.html

2. [The head - meta charset, viewport, title, description, favicons](./2-index.html)

Copy the content of 1-index.html into 2-index.html

[![Image Description](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2019/11/2ba3a0d7878316de5aaa.jpg)](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2019/11/2ba3a0d7878316de5aaa.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231005%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231005T140651Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=d5d60a535be3367f129e5fdcfd9b33d4144d2c29ed2c7d2df4c68ec5c920d87a)


* Meta charset:

* add a meta tag inside the head:
*	add the charset attribute with the value utf-8

**Viewport:**

* add a meta tag inside the head:
*	add an attribute name on the tag and specify that it is the meta viewport
*	add the key width with the value device-width
* 	add the key initial-scale with the value 1.0
*	add the key viewport-fit with the value cover

**Title:**

add the title tag just after the meta viewport with value: Homepage - Techium

**Description:**

* add a meta tag inside the head section
*	add an attribute name on the tag and specify that is the meta description
*	add another attribute called content
*	add the following description: Techium is a digital agency

**Favicons:**

* download the image above to use as a favicon
* Use the tool at https://realfavicongenerator.net/ to generate all the favicon formats
* take the favicon.ico and favicon.png and place these at the root of your project directory, so that it is siblings with your [0-9]+-index.html files.
* inside the head, create 2 link tags with these 3 attributes: rel, type, and href.
*	the first link tag:
*		rel: icon
*		type: image/x-icon
*		href: ./favicon.ico
*	the second link tag:
*  	 	rel: icon
* 		type: image/png
*	 	href: ./favicon.png


**Repo:**

* GitHub repository: alx-frontend
* Directory: 0x00-html_advanced
* File: 2-index.html

3.[ Simple header, main, footer](./3-index.html)

Copy the content of 2-index.html into 3-index.html

**Header:**

* create the header of your page between the open and close body tag
*	put the text Header inside the header

**Main:**

* create the main tag after the header tag
*	put the text Main content inside your main tags

**Footer:**

* create the footer tag after the main tag
*	put the text Footer inside the footer tags

**Repo:**

* GitHub repository: alx-frontend
* Directory: 0x00-html_advanced
* File: 3-index.html

4. [Aside](./article.html)

Copy the contents of 3-index.html into article.html

* change the title to put: Article - Techium
* inside the main tags
*	after the text, create the aside tags with text Aside

**Repo:**

* GitHub repository: alx-frontend
* Directory: 0x00-html_advanced
* File: article.html

5. [Section](./5-index.html)

Copy the content of 3-index.html into 5-index.html

* inside your <main> section
*	remove the text in main, create these sections:

1. create first section and put the text Hero section inside
2. create second section and put the text Services section inside
3. create third section and put the text Works section inside
4. create fourth section and put the text About section inside
5. create fifth section and put the text Latest news section inside
6. create sixth section and put the text Testimonials section inside
7. create seventh section and put the text Contact section inside
Does not need to pass W3C

**Repo:**

* GitHub repository: alx-frontend
* Directory: 0x00-html_advanced
*  File: 5-index.html

6. [Work, News, Testimonial articles ](./6-index.html)

Copy the content of 5-index.html into 6-index.html

**Work articles:**

* inside the section Works section
*	add 3 article tags
*		inside each article write Work # where the hashtag will be the ordered number (1, 2, or 3)

**News articles:**

* inside the section Latest news section
*	add 3 article tags
*		inside each article write Article # where the hashtag will be the ordered number (1, 2, or 3)

**Testimonial articles:**

* inside the section Testimonials section
*	add 3 article tags
*		inside each article write Testimonial # where the hashtag will be the ordered number (1, 2, or 3)

W3C won’t pass - you can ignore it

**Repo:**

* GitHub repository: alx-frontend
* Directory: 0x00-html_advanced
* File: 6-index.html

7. [Navigation](./7-index.html)

Copy the content of 6-index.html into 7-index.html

* remove the Header text inside the <header>
* create the nav tag inside the header tag
*	it should remain empty for now

**Does not need to pass W3C**

**Repo:**

* GitHub repository: alx-frontend
* Directory: 0x00-html_advanced
* File: 7-index.html

8. [Level 1 headings](./8-index.html)

Copy the content of 7-index.html into 8-index.html

* create the level 1 heading inside your main before your sections
*	put text Homepage in your heading tag

**Does not need to pass W3C**

**Repo:**

* GitHub repository: alx-frontend
* Directory: 0x00-html_advanced
* File: 8-index.html

9. [Level 2 headings ](./9-index.html)

Copy the content of 8-index.html into 9-index.html

* in the section tag with the the text Hero section, remove the text and create a level 2 heading with text We help you build your brand!
* in the section tag with the the text Services section, remove the text and create a level 2 heading with text Services
* in the section tag with the the text Works section, remove the text and create a level 2 heading with text Works
* in the section tag with the the text About section, remove the text and create a level 2 heading with text About Us
* in the section tag with the the text Latest news section, remove the text and create a level 2 heading with text Latest news
* in the section tag with the the text Testimonials section, remove the text and create a level 2 heading with text Testimonials
* in the section tag with the the text Contact section, remove the text and create a level 2 heading with text Contact

W3C won’t pass - you can ignore it

**Repo:**

* GitHub repository: alx-frontend
* Directory: 0x00-html_advanced
* File: 9-index.html

10. [Level 3 headings](./10-index.html)

Copy the content of 9-index.html into 10-index.html

**Services headings:**

* Inside the section containing the h2 heading Services, add these elements right after the h2:
*	create a level 3 heading with text Design & Concept
*	create a level 3 heading with text Digital Strategy
*	create a level 3 heading with text Content Strategy
*	create a level 3 heading with text UX Design
*	create a level 3 heading with text Web Development
*	create a level 3 heading with text Social Media

* Works headings:

* Inside the section containing the h2 heading Works:
*	in the first article, replace the text with a level 3 heading with text Interior Design
*	in the second article, replace the text with a level 3 heading with text Web Development
*	in the third article, replace the text with a level 3 heading with text Personal Brand

**About Us headings:**

* Inside the section containing the h2 heading About Us, after the h2 heading, create these elements in this order:
*	a level 3 heading with text Who are we
*	a level 3 heading with text Our culture
*	a level 3 heading with text How we work

**Latest news headings:**

* Inside the section containing the h2 heading Latest news:
* 	in the first article replace the text with a level 3 heading with text Hoc loco tenere se Triarius non potuit.
*	in the second article replace the text with a level 3 heading with text Ut alios omittam, hunc appello, quem ille unum secutus est.
*	in the third article replace the text with a level 3 heading with text Bestiarum vero nullum iudicium puto.

**W3C does not need to pass here**

**Repo:**

* GitHub repository: alx-fronte
* Directory: 0x00-html_advanc
* File: 10-index.html
