August 24, 2025
Monday

I am working on a this project, making a blog page to test and apply what I have learned so far in learning program.

I am make this documentation to document the build from every step in building it. I will try to document the entire process, how I did it and what I do, what I get right and all the issue down to that fixes.

Stage 1 - step 1

I am making the file tree for the website. Currently I am naming the root folder "personal-blog" but will change it soon that is the appropriate name for this project.

Steps:

1. Open the terminal:
   win + r
2. Changing the directory from the root directory:
   cd desktop (.\Desktop\)
3. Inside the desktop directory I made the root folder:
   mkdir personal-blog
4. Then I change the directory to 'personal-blog' and once I am inside I made the sub-folders, index.html, style.css, and README.md files. The process:
   mkdir css
   mkdir images
   mkdir post
   ni index.html
   ni styles.css
   ni README.md
5. I navigated the root file by using cd to check everything, and use ls to see all the content inside the folder:
   cd filename
   cd ..
   ls
6. I use explorer to open the entire file to further confirm that everything:
   explorer .\personal-blog\
   note: When I use explorer I change to the directory where the file is stored so that I can open it directly. It is easier to open the file when you are inside the directory and you don't need to know or write down the entire file tree.
7. After that I open the project with CS code:
   code .
   note: When I 'code .' I am inside the root file of the folder that I am opening.

The file tree for the project is this:

personal-blog
I
I--- css/
-------I-- styles.css
I
I--- images/
I
I--- posts/
I
I-- index.html
I
I--README.md

Stage 1 - step 2

HTML

This is the structure of my page/site/blog. My aim at the moment is that I will build the structure on what will be the content of the page and later when I am at CSS I will style them.

In making a page, site or in this case a blog the challenge is not just the tags, elements, or the structure that will in it but the content that will actually go inside the blog. I am thinking and doing research on what and how the content will be displayed. Just by thinking what should go in the main context and section is a challenge. The elements that I will be using will be a lot easier if I have make a plan in mind on how the blog page will look like.

Process in making the first step of this challenge:

1. I open the index.html file inside VS code.
2. The lines of code I wrote there are these:
   <!DOCTYPE html> <!-- this to determine that I am using html 5 -->
   <html lang="en"> <!-- this the language that I am using -->
   <head>
   <meta charset="UTF-8"> <!-- this the character set of code and it will be understood by other programs -->
   <meta name="viewport" content="width=device-width", initial-scale=1.0"> <!-- this for mobile responsiveness, I want the site to be accessible through different devices -->
   <title>My Blog</title> <!-- this is the title of the page and it is displayed on the browser tab -->
   </head> <!-- the head element contains the metadata and what is the page is all about but is not visible on the browser when it opened -->
   <body> <!-- body element contains all that is visible on the browser when the page is opened -->
   <h1>Welcome to My Blog</h1> <!-- is the header and h is the main header, there are 6 header types and h1 represents the main heading/title of a page or section of content.. h1 - h6. -->
   <p>This is my personal space on the web.</p> <!-- is the paragraph element. This where you write your content. -->
   </body>
   </html>
3. I save the file by using ctrl + s
4. In loading or opening the page I use the Live Server extension and use the command alt + L + alt + O

Notes:
The element must have an opening and closing tag <></>.
I have already added extensions on my VS code: Live Server, Prettier, Material Icon Theme, Auto Rename Tag, Code Spell checker, Error Lens, etc. I made the research on this when I was first starting learning HTML.
I have some basic knowledge on HTML and some CSS through reading books, video tutorials on YouTube, and having LLMs build me learning materials to use.
I applied what I have learned so far.

August 26, 2026
Stage 1 - step 3

I haven't done any entry here but I was able to do some of the structure for the semantics of the page. I basically opted for the common route but as the day goes and giving it much thought I am going to change it towards, for me is the right structure. I will change the file tree or update it towards the actual structure of this site. I will write down the initial filesystem here and with the updated filesystem and semantic structure.

Initial filesystem:

Root (personal-blog)
│
├─css/
│ └─styles.css
│
├─images/
│
├─posts/
│
├─index.html
│
└─README.md

Initial semantic structure:

<!DOCTYPE html>
<html lang="en">
<head>
	<meta>
	<title></title>
</head>
	<body>
	  <header>
	     <p></p>
		<nav class="navbar">
			<ul>
			 <li></li>
			 <li></li>
			 <li></li>
			 <li></li>
			 </ul>
		</nav>
</header>
<main class="hero">
	<img src="#" alt="#"/>
	<div class="hero-content">
	<h1></h1>
	<p></p>
	</div>
</main>
<section class="article-list">
	<article></article>
	<article></article>
	<article></article>
</section>
<footer>
	<p><a href="#"></a></p>
</footer>
</body>
</html>

Notes:
I put the class to the elements that I want to I want to organize and style when I will do CSS. I cluster them according to where I want to group them. I didn't use div to the tags or elements that are semantic and only use it in the hero section (main).

August 27, 2026
Stage 1 - step 3

Filesystem update:
Root (personal-blog)
│
├─assets/
│ ├─css/
│ │ └─styles.css
│ │
│ └─images/
│
├─posts/
│
├─index.html
├─blog.html
├─about.html
├─projects.html
│
└─README.md

Updated semantics:

<!DOCTYPE html>
<html lang="en">
<head>
	<meta>
	<title></title>
</head>
	<body>
	  <header>
	     <p></p>
		<nav class="navbar">
			<ul>
			 <li><a></a></li>
			 <li><a></a></li>
			 <li><a></a></li>
			 <li></li>
			 </ul>
		</nav>
</header>
<main>
	<img id="hero-image" src="#" alt="#"/>
	<div class="hero-content">
	<h1></h1>
	<p></p>
	</div>
</main>
<section class="overview-card">
	<h2></h2>
	<p></p>
</section>
<footer>
	<p><a href="#"></a></p>
</footer>
</body>
</html>

Notes:
This is my updated filesystem and semantics. There are comments on my code base to see my reasoning.
I use the terminal in making the new directory inside VS code; use ctrl + shift + ` to open it. in making the directory/folder I use "mkdir" then the filename. In moving the files I use "mi" filename and the file folder name to where I want to move it. In making my other .html file for the other pages I use "ni" filename.

August 28, 2026
Stage 1 - step 3

Why is this inside <main>?
It is inside my <main> because it is the main content of the home page.

Why is this a <section>?
The first section on the main element is the hero section. It contains a brief introduction of the page, like a greeting. And , the section of the main is the overview section and it will describe the content of the entire site is all about.

Why is this an <article>?
In the current page that we are building doesn't contain an article element. I don't have reusable composition, self-contained, and independent content. This is reserve for the blog.html.

Why did I use <div> here?
I use `<div>` as a generic container to group the introductory elements because the group does not require a more specific semantic container. The `<h1>` and `<p>` still have their own semantic meaning. The `<div>` will also allow me to control their layout and styling together with CSS.

Why does this have a class?
The class attribute is to label the section or areas that will be targeted, it is an identifier for me for the behavior categories to the elements and for assigning styles with CSS.

Why does this have an id?
An id is a unique identifier and identify one unique element.

Why doesn't this element need a class or id?
It depends on the element wither you will use an id or class. Id is for a unique identity of a particular element. And, class is use if the element belong to a category or group.

<body>
│
├── <header>
│   ├── site name
│   └── <nav>
│
├── <main>
│   │
│   ├── <section>
│   │   ├── hero image
│   │   └── introductory content
│   │
│   └── <section>
│       ├── overview heading
│       └── overview content
│
└── <footer>

HTML element
↓
"What does this content mean?"
↓
Semantic structure

class
↓
"What category does this element belong to?"
↓
Reusable identification / styling hook

id
↓
"Which unique element is this?"
↓
Unique identification

div
↓
"I need a generic container."
↓
Grouping without adding semantic meaning

CSS
↓
"How should all of this look?"

Updated semantics:

<html>
  <body>
    <header>
      <p></p>
      <nav >
        <ul>
          <li><a></a></li>
	  <li><a></a></li>
        </ul>
      </nav>
    </header>
    <main>
      <section>
        <img  src="" alt="." />
        <div class="intro-text">
          <h1></h1>
          <p></p>
        </div>
      </section>
      <section>
        <h2></h2>
        <p></p>
      </section>
    </main>
    <footer>
      <p><a href=""></a></p>
    </footer>
  </body>
</html>

Note: I only write the body or it is like generic or a boiler plate that I made with the semantic structure, this is just use to represent how the code will look. I will have the actual code in a different file.
