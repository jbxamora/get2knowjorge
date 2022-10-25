# get2knowjorge
A portfolio of my work throughout my Full Stack Course
# Code Refactor

## Description

This is a refactor of the Horiseon Webpage to follow accessability standards. This refactor also optimizes the webpage for search engines. Through this repo you can view changes made to the website that make it more accessible to readers. 

### User Story
```
AS A marketing agency
I WANT a codebase that follows accessibility standards
SO THAT our own site is optimized for search engines
```
### Acceptance Criteria
```
GIVEN a webpage meets accessibility standards
WHEN I view the source code
THEN I find semantic HTML elements
WHEN I view the structure of the HTML elements
THEN I find that the elements follow a logical structure independent of styling and positioning
WHEN I view the image elements
THEN I find accessible alt attributes
WHEN I view the heading attributes
THEN they fall in sequential order
WHEN I view the title element
THEN I find a concise, descriptive title
```

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [License](#license)
4. [Badges](#badges)
5. [Features](#features)
6. [Contributing](#contributing)

## Installation
No need to install applications to view the changes made. You can view the webpage by visitng the link below. 

[View Webpage](https://jbxamora.github.io/code-refactorizationinator/)

## Usage

While there are no noticable changes here are some things you want to look out for.
### Accessability
#### NavBar 

A NavBar Implemented into the website so that users are able to quickly jump from section to section.

![Picture of Nav bar](assets/images/navbar.png)

#### Keyboard Accessability 
One of the accessability standards goes over users main source of browsing a webpage being a keyboard. 
Using the tab button on you keyboard you can navigate throughout the webpage. 

![NavBar Tab Access](assets/images/navbartab.png)

#### Comments
For those that are looking inside the backend of a webpage, I've added comments to make reading through the html/css easier. 

![HTML Comments](assets/images/comments.png)

### Changes Made

#### HTML

One of the first changes that was made was the implementation of semantic HTML.
The latest commit reflects this change, you can see that we moved away from "div" elements that structure header,main,body,footer elements. For example:

```html
 <div class="hero"></div>
    <div class="content">
        <div class="search-engine-optimization">
```

The converted HTML now follows semantic order. Example:

```html
<header class="header">
        <h1>Hori<span class="seo">seo</span>n</h1>
        <nav>
```

Another Issue with the HTML was the sizing of fonts within the Benefits Area.
This made the text very hard to read. 

```html
<h3>Cost Management</h3>
```
Although it is an extremely simple fix, I beleive this change will make the website more accessable to all types of readers. Simply changing the font size can have drastic impact wether or not the user can properly view the information.

```html
<h2>Cost Management</h2>

Another small but noticable change was the Title element for the website. This lets readers know what webpage is behind the tab.

![TABTITLE](assets/images/tabtitle.png)

Lastly in HTML there was a bug that caused one of the links to break. Users would not be able to click the link and have it direct them to the correct article on the webpage. 

```html
<div class="search-engine-optimization">
```

This was a simple fix but could of been a major flaw if it wasn't caught.

```html
<section id="search-engine-optimization" class="search-engine-optimization">
```
#### CSS
The changes to the CSS file reflect my need for it to be reader friendly and add a simple but significant twist to the webpage style.

The first look at the CSS you can see a long page of CSS and at first glance it may seem intimidating but when you notice you can merge some code its an easy fix. My biggest and main change to the CSS was consolidating the code to make it less intimidating for readers. This also includes adding comments that give simple descriptions about where you are in reference to the HTML file.

```CSS
.search-engine-optimization img {
    max-height: 200px;
}

.online-reputation-management img {
    max-height: 200px;
}

.social-media-marketing img {
    max-height: 200px;
```

After consolidation the code now looks like this. Not as intimidating and easy to read.

```CSS
  .search-engine-optimization img, .online-reputation-management img, .social-media-marketing img {
    max-height: 200px;
}
```
The last change to the CSS file was something I learned in class and have been waiting to implement. A hover feature!
While this might not seem exciting I took into consideration that the 'SEO' in HORISEON stood for Search Engine Optimization. I noticed that those letters were an acronym and wanted to capitalize on that information. 

![SEO Hover Model](assets/images/hoverseo.png)

Here is the underlying code if you want to add it to a future project.

```css
.header h1 .seo {
    color: #d9dcd6;
}

.header h1 .seo:hover {
    color: black;
    transition: all .7s linear;
}
```

## License

MIT License

Copyright (c) [year] [fullname]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Badges

<a href=”https://www.linkedin.com/in/jorge-zamora-786945250/”>
<img src='https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=linkedin&labelColor=blue'>

![badmath](https://img.shields.io/github/followers/jbxamora?label=JBXAMORA&logoColor=%23fd2423&style=social)

![badmath](https://img.shields.io/github/license/jbxamora/code-refactor)

## Features

1. HTML
2. CSS
3. GitHub
4. LiveSite
5. Accessability
6. Hover 
7. Comments

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. If the issue goes unresolved for more than a week feel free to contact me at any of the links listed below. Be sure to add me on LinkedIn and Follow me on GitHub to view my course progression.

[<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/github.svg' alt='github' height='40'>](https://github.com/jbxamora)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/linkedin.svg' alt='linkedin' height='40'>](https://www.linkedin.com/in/jorge-zamora-786945250//)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/instagram.svg' alt='instagram' height='40'>](https://www.instagram.com/jbxamora/)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/stackoverflow.svg' alt='stackoverflow' height='40'>](https://stackoverflow.com/users/20023706/jbxamora)