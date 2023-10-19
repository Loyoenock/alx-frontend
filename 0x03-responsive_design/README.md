# 0x03. Responsive design

__HTML | CSS | Front-end | Responsive design__

## Resources

__Read or watch:__

* [The building blocks of responsive design - Progressive web apps | MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)
* [A pragmatic guide to designing and building responsive web applications | developerlife.com](https://developerlife.com/2019/08/25/guide-to-building-responsive-web-apps/)
* [Understanding the difference between mobile-first, adaptive and responsive design](https://fredericgonzalo.com/en/understanding-the-difference-between-mobile-first-adaptive-and-responsive-design/)
* [LukeW | Mobile First](https://www.lukew.com/ff/entry.asp?933)
* [Media Queries | A collection of inspirational websites using media queries and responsive web design](https://mediaqueri.es/)
* [Responsive Design Newsletter](https://bytes.dev/?s=rwd)

## Learning Objectives

At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/), without the help of Google:

* Mobile-first design
* Media-queries
* Sizes to use for responsive web design
* How to make a website responsive
* The differences between responsive and adaptive design
* CSS units that are used to make elements flexible

##Requirements

* Allowed editors: vi, vim, emacs
* A README.md at the root of the project directory is mandatory
* HTML and CSS have been rendered on Chrome 78 or more.


### Wireframe of the Techium project - mobile version

![Wireframe](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/4/a1f906a6a39eba8cb2f3d2877abc9ea84be51d9d.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=9b3dfe1ddc56010968f2f42b1ea93c6ff75dd3af4ef0d559ff401bfc9afa62d1)

### Starter files

* 00-index.html
* 00-styles.css


### Tasks

0. [Fix the hero banner](./01-styles.css, 01-index.html)
Because we did some changes with the article.html page in the previous project, our hero banner background is no more visible. Let’s fix it!

But before that, to ensure we start on the same foot, you should use the starter HTML and CSS provided in the project description.

In your 01-styles.css file

* Inside the hero-homepage class selector, update some values:
*   Property: background-position, Value: 65% 8rem
*   Property: background-size, Value: 90rem auto
* Inside the selector that targets section-inner class inside section-hero class
*   Update the min-height to 35vh

__Final rendering of the Hero section should look something like this__

![Hero](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/f464d8346c36134ec4ae.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=dc26c8629de0fbec02c26316a4462966edf17b2848fab05a5364ee6e449d2d95)


__Repo:__

* GitHub repository: alx-frontend
* Directory: 0x03-responsive_design
* File: 01-styles.css, 01-index.html

1. [Make the container flexible](./02-styles.css, 02-index.html)

Using the previous file as the base, in your 02-styles.css file update the .container selector by changing width to max-width

If you resize your browser, you should see that the content is resizing.

Wide screen:

![Container](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/5356d9d9b1de3ef692a1.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=7408074778e0d514b35c8f89c597d9c7c2bbe6fb837179d13603308c9ce278ff)

Narrow screen:

![Container](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/9aeb51d5b4c9586ea05a.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=aa317c2932701458abfca5685169b19d608734649be672d91720755f8a64af16)

__Repo:__

* GitHub repository: alx-frontend
* Directory: 0x03-responsive_design
* File: 02-styles.css, 02-index.html

2. [Fix layout issues](./02-1-styles.css, 02-1-index.html)

Whatever the browser you use, it’s a good idea from now on, to toggle the device view.

In a normal situation, you should start with “mobile first” in mind and write your CSS first for the mobile. But because we already have a desktop version, we will exceptionally add some media-queries for mobile and tablet.

* For extra large devices (no media queries)
* For desktop / large devices (max-width: 992px)
* For tablet / medium styles (max-width: 767px)
* For mobile styles (max-width: 480px)

__We will put media queries at the end of each section to facilitate the reading but for performance reasons, the best practice is to unifiy all similar breakpoints at the end of the CSS file.__

In your 02-1-styles.css file:

* inside the /\* Helpers section target all images inside the main section

*   Property: width, Value: 100%
*   Property: height, Value: auto

* inside the /\* Section Latest news section, add a new media query (max-width: 767px)

*   Target the row inside section-latest-news
*       Property: flex-direction, Value: column
* inside the /\* Grid section, at the end, add a new media query (max-width: 767px)

*   First, redefine the variable section-padding and give that value: 5rem 1.5rem. And redefine the variable section-body-padding with 2rem 0 0
*   Target the ul.row and the row class
*       Property: flex-direction, Value: column
*       Property: margin, Value: 0
*   Target all the classes that started with col-
*       Property: margin, Value: 0 0 3rem 0
*   Target the col-1-3 and col-1-2 classes
*       Property: width, Value: 100%

The navbar is not allowing the website to fit the window. We will temporarily hide it and create a mobile navbar later.

* inside the /\* Navbar section, at the end, add a new media query (max-width: 767px)
*   Target the navbar-menu class
*       Property: display, Value: none
You should now be able to easily view the website on a device of any screen/window size. I guess you are surprised that was so easy?!

Rendering on wide screen

![About](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/ec686cf75a8788a04bd5.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=26249b36b4b58b4dd37c6f79c9ff92cb66346ff3b7d22d2570385e0f6ec8b229)

Rendering on screen with max-width: 767px

![Works](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/741a7a68af4e92b5c286.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=3044f88f88a548d695e9675f9f06a1235faaaa6c3f53362d7e97acc6500836bf)

Rendering on screen with max-width: 767px, you can see the navbar is hidden
![Service](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/3ee548024a868f4ce695.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=279e562199fd660bf1ff1b402ba10addac18ec203de708f85e489fa6fb5db9be)


__Repo:__

* GitHub repository: alx-frontend
* Directory: 0x03-responsive_design
* File: 02-1-styles.css, 02-1-index.html

3. [Generate images with responsive breakpoints](./03-index.html, 03-styles.css)

Go to Responsive Breakpoints

In Breakpoints generation settings:

* Resolution: From 380 to 1200
* Size step: 25
* Maximum images: 3
* Art-direction: Desktops
* Upload your images one at a time:
*   pic-about-01.jpg
    pic-article-01.jpg
*   pic-article-02.jpg
*   pic-article-03.jpg
* Copy the markup for the <img> tags and replace your current <img> tags with it.
* Download the images and place them into the images directory

Here’s an example on how to add different resolutions of the same image

```
<img
    sizes="(max-width: 3000px) 40vw, 1200px"
    srcset="
      about-us_icoxoo_c_scale,w_380.jpg 380w,
      about-us_icoxoo_c_scale,w_853.jpg 853w,
      about-us_icoxoo_c_scale,w_1200.jpg 1200w"
    src="about-us_icoxoo_c_scale,w_1200.jpg"
    alt="">
```

__Repo:__

* GitHub repository: alx-frontend
* Directory: 0x03-responsive_design
* File: 03-index.html, 03-styles.css

4. [Create the mobile icon and hide the menu](./04-index.html, 04-styles.css)

We want to have a clickable icon that shows and hide our navigation. We don’t want to use JavaScript but find a pure HTML / CSS way. We learned that input type checkbox have a checked - unchecked state. So we are going to use this for our menu.

Using the previous files as the base for this project

__Changes to the HTML__

Just before the <nav class="navbar-menu">

* Create an input (which will be not visible)

*   Class: menu-btn
*   Type: checkbox
*   Id: menu-btn

* Create a label

*   Class: menu-icon
*   For: menu-btn
*   In the label create an empty span with the navicon class.

__Changes to the CSS__

Inside the /\* Navbar section, and inside the 767px media query

* Create the root global selector. We want to override a CSS variable:

*   Variable name: nav-item-margin, Value: 0

* In the selector for the navbar-menu class

*   Property: flex, Value: 1
* Target the nav class in header class

*   Property: flex-direction, Value: column (for the element of the menu be below each other)
*   Property: overflow, Value: hidden
*   Property: max-height, Value: 0 (the display property can’t be animated, so we use the height that can be animated)
*   Property: transition, Value: max-height .2s ease-out

__Rendering on screen with max-width: 767px, the check box is the input__

![Mobile](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/17e4ace4fe8c91201e0a.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=2f008cecfec3b357e90beca9b511bb62554836ab5df186400117fca1b1bb8c07)

__Repo:__

* GitHub repository: alx-frontend
* Directory: 0x03-responsive_design
* File: 04-index.html, 04-styles.css

5. [Hamburger!](./05-index.html, 05-styles.css)

Let’s now, use a little bit of CSS magic to create an “hamburger” icon just with CSS.

Using the previous files as the base for this task:

* Target the menu-icon class inside the header class

*   Property: cursor, Value: pointer
*   Property: padding, Value: 2.5rem
*   Property: position, Value: relative
*   Property: user-select, Value: none
* Target the navicon class inside themenu-icon class which is inside the header class

*   Property: background, Value: point to the color-white variable
*   Property: display, Value: block
*   Property: width, Value: 2rem
*   Property: height, Value: .2rem
*   Property: position, Value: relative
*   Property: transition, Value: background .2s ease-out
* Target the before and after pseudo elements of the navicon class inside the menu-icon class which is inside the header class

*   Property: content, Value: empty string
*   Property: display, Value: block
*   Property: width, Value: 100%
*   Property: height, Value: 100%
*   Property: position, Value: absolute
*   Property: background, Value: point to the color-white variable
*   Property: transition, Value: all .2s ease-out
* Target only the before pseudo element of the navicon class inside the menu-icon class which is inside the header class

*   Property: top, Value: .7rem
* Target only the after pseudo element of the navicon class inside the menu-icon class which is inside the header class

*   Property: top, Value: -.7rem

__Rendering of the hamburger on max-width: 767px__

![Sercess](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/87f845e172312626e0fc.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=c2b1746a5a33062b42a3bec2c22e983d041ca94ef8ea306f18f89b6e27e081b8)

__Repo:__

* GitHub repository: alx-frontend
* Directory: 0x03-responsive_design
* File: 05-index.html, 05-styles.css

6. [Add the behavior based on menu-btn state](./06-index.html, 06-styles.css)

in your CSS file:

* Create a new comment section /* menu btn */
* Target menu-btn class inside header class
*   Property: display, Value: none
* Target navbar-menu class when the menu-btn class element is checked
*   Property: display, Value: block
*Target nav class inside navbar-menu class when the menu-btn class element is checked

*   Property: max-height, Value: 100%
*   Property: overflow, Value: inherit
* At the end of the /\* Section HERO section, create a new media query for max-width: 767px

*   Target the section-hero class
*       Property: margin, Value: -0.1rem 0
*   Target the hero-homepage class
*       Property: background-position, Value: 85% 0
*   Target the section-body class inside section-hero class
*     Property: padding, Value: 2rem

Going back to the /\* menu btn \*/ section

* Target the navicon class inside menu-icon class sibling to the menu-btn when it is checked and inside header class
*   Property: background, Value: transparent
* Target the before state of navicon class inside menu-icon class sibling to the menu-btn when it is checked and inside header class element
*   Property: transform, Value: rotate(-45deg)
* Target the after state of navicon class inside menu-icon class sibling to the menu-btn when it is checked and inside header class element
*   Property: transform, Value: rotate(45deg)
* Target the before and after states of navicon class when inside menu-icon class sibling to the menu-btn class when it is checked and inside header class

*       Property: top, Value: 0
* Create a new media query for max-width: 767px

*   Target the root and redefine the header-padding variable with 2rem 0 0
*   Target header class
*       Property: background, Value: point to the color-black variable
*   Target the header-container class
*       Property: flex-wrap, Value: wrap
*       Property: padding, Value: 0 1.5rem
*   Target the menu-icon class inside the header class
*       Property: display, Value: block
* Create a new media query for max-width: 480px

*   Target the header-logo class
*       Property: flex-basis, Value: 70%
* Create a new media query with min-width: 481px and max-width: 767px

*   Target the header-logo class
*       Property: flex-basis, Value: 79%
* Find the .header .menu-icon selector and add display: none; to hide the menu icon when we are on desktop mode.

__Rendering on screen with max-width: 767px, when the input is unchecked the menu is not displayed__

![Services](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/b9f67a5f3bdfdbd4cd88.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=a77aa875b022dda14792fcec47cd1e258471cfd494d37b71e64a498645f01a7e)

Rendering on screen with max-width: 767 px, when input is checked the menu block is displayed

![Services](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/fe0ae0bfb739a19ae933.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=b43ca92df0c3defdc084eb561bb31c23f6904645db70493aae159dc7b86d7dc0VVV)

Rendering on desktop screen, menu icon is not visible

![Services](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/aa52c972d075f360f8bc.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=f24a26bb9bda157c9a7affb024840bd5f54dee803e7173ebdcb6cb98295a05c5)

__Repo:__

* GitHub repository: alx-frontend
* Directory: 0x03-responsive_design
* File: 06-index.html, 06-styles.css

7. [Make the font size responsive](./07-index.html, 07-styles.css)

We have multiple ways to make the typography responsive. The basic way would be to create multiple media queries and set a different font-size. But because we are using REM that are based on 62.5% (defined in the html selector). Changing that value would change proportionally all font sizes.

In your CSS file at the end of the /\* Base section

* Create a new media query for max-width: 480px
*   Target the html element
*       Property: font-size, Value: 57%
* Create a new media query for min-width: 481px and max-width: 767px
*   Target the html element
*       Property: font-size, Value 60%

This is a simple way to achieve responsive typography. More complex options can also be used to have a more granular control over the font sizes.

__Repo:__

* GitHub repository: alx-frontend
* Directory: 0x03-responsive_design
* File: 07-index.html, 07-styles.css

8. [Improve the "Works" section](./08-index.html, 08-styles.css)

in 08-styles.css, at the end of the /\* Card WORK

* Create a new media query of max-width: 767px
*   Target the card-inner class inside the card-work class
*       Property: variable called text-color, Value: point to color-white variable
*       Property: position, Value: relative
*   Target the card-title class inside the card-work class
*       Property: opacity, Value: 1
*   Target all a tags inside .card-work .card-title class:
*       Property: padding, Value: 2rem 1rem 0 1rem

__Rendering on screen of max-width: 767px__



__Repo:__

* GitHub repository: alx-frontend
* Directory: 0x03-responsive_design
* File: 08-index.html, 08-styles.css
 
9. [Improve the "Footer" section](./09-index.html, 09-styles.css)

in 09-styles.css, in the /\* Footer section

* Create a new media query of max-width: 767px.
*   Create the root global selector. We want to override a CSS variable:
*       Variable name: footer-padding, Value: 5rem 2rem 1rem
*   Target .social.nav inside the footer class and the footer-nav class inside the footer class
*       Property: text-align, Value: center
*   Target the adjacent lito the li inside the .social.nav and the adjacent li to the li inside .footer-nav (to easily add a left padding starting on the second li)
*       Property: padding-left, Value:2rem

__Rendering on screen of max-width: 767px__

![Footer](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/a12e272db34a9c4e47e9.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=2ddac3ea17e64c90cea05c5fcd0e5f93c2aa48c667a1229f1ac549cb532d8796)

__Repo:__

* GitHub repository: alx-frontend
* Directory: 0x03-responsive_design
* File: 09-index.html, 09-styles.css

10. [Fix the top header background](./10-index.html, 10-styles.css)

In 10-index.html, in the body tag, add the class article-page

In 10-styles.css, in the /\* Section HERO section, just before the media query:

* Target section-hero class inside article-page class
*           Property: margin-top, Value: -8.5rem
*       Property: padding-top, Value: 5rem

__Rendering of header and section-hero class elements__

![header](./https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/2/7a38d40512c0c6edb211.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20231018%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20231018T174110Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=7cf838859989bac2f2960af0529610bf29ef139ce5fad75e764c5ca264e7e2c5)

__Repo:__

* GitHub repository: alx-frontend
* Directory: 0x03-responsive_design
* File: 10-index.html, 10-styles.cs
