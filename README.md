# code-refractor-homework 


## View the deployed file @  https://mambasnow.github.io/code-refractor-homework/

For this file changes were made to the original Horiseon website. 
Changes include:
                *Cleaning CSS
                *Adding Semantics to html  (Section, Aside, footer, header , Navbar)
                * Fixing link and fixing corrolating classes and IDs in html
                * adding notes for future developers



## CSS Changes 

Original Css was cluttered with a lot of repeating code that applied to several IDS under the content div
To make easier readablility we changed it from  adding the css to its indivual IDs to cover all matching css to
its respective overall sections. 

>  {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}

body {
    background-color: #d9dcd6;
}

.header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}

.header h1 {
    display: inline-block;
    font-size: 48px;
}

.header h1 .seo {
    color: #d9dcd6;
}

.header div {
    padding-top: 15px;
    margin-right: 20px;
    float: right;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 20px;
}

.header div ul {
    list-style-type: none;
}

.header div ul li {
    display: inline-block;
    margin-left: 25px;
}

a {
    color: #ffffff;
    text-decoration: none;
}

p {
    font-size: 16px;
}

.hero {
    height: 800px;
    width: 100%;
    margin-bottom: 25px;
    background-image: url("../images/digital-marketing-meeting.jpg");
    background-size: cover;
    background-position: center;
}

.float-left {
    float: left;
    margin-right: 25px;
}

.float-right {
    float: right;
    margin-left: 25px;
}

.content {
    width: 75%;
    display: inline-block;
    margin-left: 20px;
}

.benefits {
    margin-right: 20px;
    padding: 20px;
    clear: both;
    float: right;
    width: 20%;
    height: 100%;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #2589bd;
}

.benefit-lead {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-brand {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-cost {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-lead h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-brand h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-cost h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-lead img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

.benefit-brand img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

.benefit-cost img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

.search-engine-optimization {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}

.online-reputation-management {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}

.social-media-marketing {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}

.search-engine-optimization img {
    max-height: 200px;
}

.online-reputation-management img {
    max-height: 200px;
}

.social-media-marketing img {
    max-height: 200px;
}

.search-engine-optimization h2 {
    margin-bottom: 20px;
    font-size: 36px;
}

.online-reputation-management h2 {
    margin-bottom: 20px;
    font-size: 36px;
}

.social-media-marketing h2 {
    margin-bottom: 20px;
    font-size: 36px;
}

.footer {
    padding: 30px;
    clear: both;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    text-align: center;
}

.footer h2 {
    font-size: 20px;
}



## New CSS

This css is more readable and easier to locate the sections and families in which it belongs to

>* {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}

body {
    background-color: #d9dcd6;
    font-size: 16x;
}

header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}

header h1 {
    display: inline-block;
    font-size: 48px;
}

/* Changes the "SEO" latters in header according to story */
#seo {
    color: #d9dcd6;
}
/* Main container for  navagation bar on the top of page  */
 .nav-bar {
    padding-top: 15px;
    margin-right: 20px;
    float: right;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 20px;
}

 .nav-bar ul {
    list-style-type: none;
    
}
/* Setting display for nav list elements to be in-line */
 .nav-bar ul li {
    display: inline-block;
    margin-left: 25px;
}

a {
    color: #ffffff;
    text-decoration: none;
}

#Banner {
    height: 800px;
    width: 100%;
    margin-bottom: 25px;
    background-size: cover;
    background-position: center;
}
/* puts images to the left size of a div */
.float-left {
    float: left;
    margin-right: 25px;
}


/* puts images to the right size of a div */
.float-right {
    float: right;
    margin-left: 25px;
}


/*Main content container on the left side  */
.content {
    width: 75%;
    display: inline-block;
    margin-left: 20px;
}
/* Sets all h2 in content properties*/

.content h2{
    margin-bottom: 20px;
    font-size: 36px;
}

/* Sets properties for the main section called benefits */
.benefits {
    margin-right: 20px;
    padding: 20px;
    clear: both;
    float: right;
    width: 20%;
    height: 100%;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #2589bd;
    color: #ffffff
}
/* Properties for summary divs in benifits  making sure theres room below the div boxes */
.benefits summary {
    margin-bottom: 32px;
}



.benefits h3{
    margin-bottom: 10px;
    text-align: center;
}
/* Setting all image elements with the class name "benefits-img" in benefits to be the same size  */
.benefits-img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}


.content summary
 {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}

.content summary img  {
    max-height: 200px;
    display: block !important;
}

/* Footer container at the bottom of the page */
footer {
    padding: 30px;
    clear: both;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    text-align: center;
}

footer h2 {
    font-size: 20px;
}




## HTML Semantics

Original html had no semantics hard to navigate and locate around 
So we changed the divs to appropriate semantic tags to help the reviewers of code


* Header 
* Nav for the nav bar
* Content 
* Summary
* (Section) under summary Div
* Aside Bar
* Section under aside 





## Nav Links now all go to the correct section

There was a single link in the nav bar that didn't  work "search-engine-optimization" link. This shouldve routed the user to the section in main content
Because the link was tied to a ID it did not go because the section engine optimization was classified as a CLASS. 

We changed this to and ID instead.


