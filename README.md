# Unit 3 Challenge: Code Portfolio Wireframe

In week one, you started laying the groundwork for your portfolio by designing a wireframe. This week we will continue to work on your portfolio by coding it using HTML & CSS.

An online portfolio is essential to transitioning to a new career in front-end development. Your online portfolio communicates who you are and your work! A portfolio is also a place to practice iterating and applying your growing UX, UI, and front-end web design skills.

## Instructions

### Step 1: Redline Your Wireframe

As a front-end developer, the first thing we do is strategically plan out how we want to code a page. We do that by redlining a wireframe or mockup given to us by the design team. 

Before you begin coding, you should mentally map out what HTML tags you need to use. Open Figma and open your About Me wireframe page.

* If you don't want to use your wireframe, feel free to use one of the [Portfolio Wireframe Templates](https://www.figma.com/file/tWUFrolsmX46u4baIzaJDC/Portfolio-Wireframe-Template?node-id=0%3A1)

* Create three new artboards and redline the following sections.

    * Your header section

    * Your hero image section.

    * Your footer section.

* Redline your header section. Your header should contain the following tags:

    * A `header` tag
    * An `img` tag
    * A `p` tag
    * A `ul` tag
    * Four `li` tags containing the text: 
        * About
        * Skills
        * Work
        * Contact

Header Example

![Image](Images/01.png)

* Redline your hero image section. Your hero image should contain the following tags:

    * A `section` tag
    * A `div` tag that is wrapped by the section tag
    * An `img` tag wrapped inside the div
    * An `h1` tag wrapped inside the div
    * A `p` tag wrapped inside the div
    * A `button` tag wrapped inside the div

Hero Image Section Example

![Image](Images/02.png)

* Redline your footer section. Your footer section should contain the following tags:

    * A `footer` tag
    * A `ul` tag
    * Four `li` tags that contain the following text:
        * About
        * Skills
        * Work
        * Contact

Footer Section Example

![Image](Images/03.png)

### Step 2: Export assets from your Figma

* Open the design file you created during unit 1 where you designed a wireframe of an About Me page using Figma.

* Export the following assets using Figma into your images folder. 

    * An image of yourself
    *Your logo

* Make sure you save the images in the images folder you created in the previous step.

![Image](Images/04.png)

### Step 3: Create and clone a GitHub repository to your desktop

* Navigate and login to www.GitHub.com and click new in the top left of github.com.

![Image](Images/05.png)

* Create a new GitHub repo in GitHub named `HW_3_My_Portfolio`.

* Clone the empty repo to your local computer.

* Create the proper folder structure inside `HW_3_My_Portfolio` to hold your website assets.  Review the folder structure in the following screenshot for a good example. 

* Create two folders inside our `HW_3_My_Portfolio` folder that you just cloned to the code folder on your desktop. Name the first folder CSS. Name the second folder images.

* Open `Visual Studio Code`.

* Add your code folder to a visual studio workspace. Click file -> add folder to workspace.

![Image](Images/07.png)

Create an `index.html` file in your root folder and an `style.css` file located in your CSS folder (illustrated below) using VSCode. 

![Image](Images/06.png)

### Step 4: Create a basic HTML structure for a navbar, hero image, and footer

To practice being a front-end developer, let’s start coding in our GitHub repository using Visual Studio Code. 

Open the `index.html` file you created in Visual Studio Code.

Create the basic HTML structure for our HTML document.

![Image](Images/10.png)

Inside the `<body>` tag, create the following `<div>` tags to hold our content.

Let's create some navigation

1. A `<header>` tag with the class of `navigation`. Create the following HTML structure inside of it: 
    
    - A `<div>` tag with the class of `inline-block` and `logo`. 
        - Wrapped inside this div tag, create an: `<Img>` tag with a `logo`. 
        - Use the image of your logo you exported during the second step of this homework. If you don't have a logo use: https://placehold.co/150x100/png

2. A `nav` tag with the class of `inline-block`. Wrapped inside of the nav tag create:
- An `unordered list tag` that wraps `four li tags`.
    - Give the li tags the class of `inline-block`. 
        - Inside your first li tag, add the text “about.”
        - Inside your second li tag, add the text “skills.”
        - Inside your third li tag, add the text “work.”
        - Inside your fourth li tag, add the text “contact.”

Code the hero image HTML:

1. Under your header, create a `<section>` tag with the class of `heroImg`.

2. Wrapped inside the hero image section, create:

- A `<div>` with the class of `content`. Inside this div, create the following HTML structure:
    - An `<img>` tag with a picture of yourself.
    - A `<p>` tag that contains a paragraph about yourself!
    - A `<button>` tag with the words “Download Resume.”

Code the footer HTML:

1. Under your section with the class of `heroImg` create a `<footer>` tag.
2. Wrapped inside the footer section create:
- An `<ul>` tag that wraps four `<li>` tags.
    - Give the `li` tags the class of `inline-block`. 
        - Inside your first li tag, add the text “about.”
        - Inside your second li tag, add the text “skills.”
        - Inside your third li tag, add the text “work.”
        - Inside your fourth li tag, add the text “contact.”

### Step 5: Attach a stylesheet and style the HTML of your navbar, hero image, and footer sections 

As a front-end developer, now that you have some HTML structure, you can select and style your elements via a CSS stylesheet.

1. In Visual Studio Code, open your `style.css` file located in your CSS folder.
2. Create a `<link>` tag to connect your HTML file to your CSS file.

Code navbar CSS:

1. First, we need all the elements to line up next to each other to build out our navbar. In our `style.css` file, create a `selector` that targets our elements with the class of `inline-block`.
- Give this `selector` the CSS property of `display: inline-block;` - this will cause our navbar to line up next to each other.
- Give this selector the property of 'vertical-align: top;' to ensure all elements align next to one another.

2. Next, we need our divs to fill the width of our container.
- Create a [CSS 'selector'](https://www.w3schools.com/css/css_selectors.asp) that targets our `<div>` with the class of `logo`.
    - Set this element’s `width to 23%`.
    - Give this element a `padding of 1%`.
- Create a CSS selector that targets our HTML element `<nav>`. If you don’t remember how to target base HTML elements, read this [documentation](https://www.w3schools.com/cssref/css_selectors.asp)
    - Set this element’s `width to 73%`.
    - Give this element a `padding of 1%`.

3. Let’s align our unordered list in its container to the right.
- Target the base HTML `<ul>` element we created earlier.
    - Give it a `width of 50%`.
    - Center it using `margin-left: auto;`.

4. Let’s center our images inside their containers also. In our CSS selector that targets the class of logo:
- Give this element the CSS property `text-align: center;`


Code hero image CSS:

1. To begin, give our `<section>` with the class of `heroImg` a height.
- Give this element the CSS property of `height: 600px;`
- Give this element `padding: 25px;`

2. Create a CSS selector that targets the class of `content`.
- Give this element `width: 500px;`
- Center this element using `margin: 0 auto;`

Code footer CSS:

1. To build out your footer, write a CSS selector that targets the base HTML `<footer>` element.
- Give this selector a `background color: #373738;`
- Use `padding` to center your `<ul>` and `<li>` elements.


2. Write a CSS selector that targets your `<ul>` nested inside of our `<footer>` element.
- Set this element to `display:inline-block;` level element.
- Give this selector the property of `vertical-align: top;` to ensure all elements align next to one another.
- Use `padding` to center the text inside of our `<li>` elements.

That’s it! We now have a basic wireframe of our portfolio site for you to practice your CSS skills on.

When you are finished styling, make sure you reupload your modified CSS files to GitHub so the world can see your work!

Here are a couple of links to some CSS properties that you can experiment with if you have time:
- https://www.w3schools.com/cssref/pr_background-image.asp
- https://www.w3schools.com/cssref/css3_pr_box-shadow.asp
- https://www.w3schools.com/cssref/pr_font_font-family.asp
- https://www.w3schools.com/html/html_colors.asp

Strategies for applying visual design to your portfolio:

- Apply `background-colors` to your `navbar` and the associated unordered lists and list items contained inside.
- Add a `background image` to your hero image. Make sure to use `background-size: cover;` and `background-repeat: no-repeat;` to make your background span your page’s full width.
- Apply a `drop shadow` to the div contained inside your hero image.
- Add a `font-family` to the text elements in your li and p tags.

### Step 6: Upload your coded website’s index.html, style.css, and images folder to GitHub and publish via GitHub Pages

As a front-end developer, getting practice publishing your work and hosting it online will not only help you submit your assignment but also get you into the habit of getting feedback and practicing using Github.

Upload your finished webpage to GitHub using GitHub.

Publish your site on GitHub Pages. If you forgot here is a [how to use gh-pages resources](https://docs.github.com/en/github/working-with-github-pages/creating-a-github-pages-site). 

Make sure you copy the URL. You will need it to submit your homework.

Congrats on creating your first portfolio website!

## Requirements

This challenge is assessed on the following criteria: 

### Technical Acceptance Criteria: 40%

* Satisfies all of the above acceptance criteria 

### Deployment: 32%

* Application deployed at live URL (if applicable).

* Application loads with no errors.

* Application GitHub URL submitted (if applicable).

* GitHub repository that contains application code.

### Application Quality: 15%

* Application resembles (at least 90%) screenshots provided in the challenge instructions.

### Repository Quality: 13%

* Repository has a unique name.

* Repository follows best practices for file structure and naming conventions.

* Repository follows best practices for class/id naming conventions, indentation, quality comments, etc.

* Repository contains multiple descriptive commit messages.

* Repository contains quality README file with description, screenshot, and link to deployed application.
---

## Copyright

© 2021 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
