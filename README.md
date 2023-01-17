# myProfessionalPortfolio

## Your Task

Welcome to this week's Challenge! This is an even-numbered week, so you won't be given any starter code. Instead, you'll create a web application from scratch! This week, you'll build a portfolio page, which you can add to as the course progresses. 

A portfolio of work can showcase your skills and talents to employers looking to fill a part-time or full-time position. An effective portfolio highlights your strongest work as well as the thought processes behind it. Students who have portfolios with deployed web applications (meaning they are live on the web) are typically very successful in their career search after the boot camp. This last point can’t be stressed enough: having several deployed projects is a minimum requirement to receive an initial interview at many companies. 

With these points in mind, in this Challenge you’ll set yourself up for future success by applying the core skills you've recently learned: flexbox, media queries, and CSS variables. You'll get to practice your new skills while creating something that you will use during your job search. It’s a win-win that you'll likely be grateful for in the future!

**Note:** If you don't have enough web applications to showcase at this point, use placeholder images and names. You can change them to real applications as you create them later in the course.

Let’s take a look at what a user story written from the perspective of a hiring manager might look like. As you might remember from your first Challenge, we follow the AS AN / I WANT / SO THAT format. 


## User Story

```
AS AN employer
I WANT to view a potential employee's deployed portfolio of work samples
SO THAT I can review samples of their work and assess whether they're a good candidate for an open position
```


## Acceptance Criteria

Here are the critical requirements necessary to develop a portfolio that satisfies a typical hiring manager’s needs:

```
GIVEN I need to sample a potential employee's previous work
WHEN I load their portfolio
THEN I am presented with the developer's name, a recent photo or avatar, and links to sections about them, their work, and how to contact them
WHEN I click one of the links in the navigation
THEN the UI scrolls to the corresponding section
WHEN I click on the link to the section about their work
THEN the UI scrolls to a section with titled images of the developer's applications
WHEN I am presented with the developer's first application
THEN that application's image should be larger in size than the others
WHEN I click on the images of the applications
THEN I am taken to that deployed application
WHEN I resize the page or view the site on various screens and devices
THEN I am presented with a responsive layout that adapts to my viewport
```


## Mock-Up

The following animation shows the web application's appearance and functionality:

![portfolio demo](./Assets/02-advanced-css-homework-demo.gif)


## Grading Requirements

> **Note**: If a Challenge assignment submission is marked as “0”, it is considered incomplete and will not count towards your graduation requirements. Examples of incomplete submissions include the following:
>
> * A repository that has no code
>
> * A repository that includes a unique name but nothing else
>
> * A repository that includes only a README file but nothing else
>
> * A repository that only includes starter code

This Challenge is graded based on the following criteria: 

### Technical Acceptance Criteria: 40%

* Satisfies all of the above acceptance criteria.

### Deployment: 32%

* Application deployed at live URL.

* Application loads with no errors.

* Application GitHub URL submitted.

* GitHub repository contains application code.

### Application Quality: 15%

* Application resembles the mock-up functionality provided in the Challenge instructions.

### Repository Quality: 13%

* Repository has a unique name.

* Repository follows best practices for file structure and naming conventions.

* Repository follows best practices for class/id naming conventions, indentation, quality comments, etc.

* Repository contains multiple descriptive commit messages.

* Repository contains quality readme with description, screenshot, link to deployed application.

## Review

You are required to submit BOTH of the following for review:

* The URL of the deployed application.

* The URL of the GitHub repository that contains your code. Give the repository a unique name and include a README file that describes the project.

- - -
© 2022 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.














<!DOCTYPE html>
<html lang="en">

<head>
    <title>Professional Portfolio</title>
    <meta charset="UTF-8"/>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link rel="stylesheet" type="text/css" href="./styles.CSS" />
</head>

<body>
    <header class="main-header">
        <h1 id="name">Jacob Maynard</h1>
        <nav>
            <a href="#">About Me</a>
            <a href="#">Work</a>
            <a href="#">Contact Me</a>
            <a href="#">Resume</a>
        </nav>
    </header>
    
    <section class="about-me">
        <h3>About me bio</h3>
    </section>

    <aside class="side">
        <h4>About Me</h1>
        <h5>Work</h2>
        <h6>Contact Me</h3>
    </aside>

    <main class="boxes">
       
        <section class="box mern">
            <header>Surf Report</header>
            <h2>MERN Stack</h2>
        </section>
        <section class="box">
            <header>LED Wall</header>
            <h2>node/iot</h2>
        </section>
        <section class="box">
            <header>Calculator</header>
            <h2>React/Javascript/CSS</h2>
        </section>
        <section class="box">
            <header>Pastel Puzzels</header>
            <h2>MERN Stack</h2>
        </section>
        <section class="box">
            <header>Run Buddy</header>
            <h2>HTML CSS</h2>
        </section>
        
    </main>
    <footer>This is footer</footer>
</body>



</html>


* {
    box-sizing: border-box;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    margin: 0;
}
.about-me{
    padding-left: 130px;
    padding-bottom: 50px;
}
/* 
main {
    display:flexbox;
    flex-wrap:wrap;
    margin-top: 2%;
    flex-direction:column;
    
} */

.main-header {
    display:flex;
    justify-content: space-between;
    padding: 60px;
    background: gray;
    color: orange;
}

.box {
    flex: 1 0 200px;
    padding: 10px;
    text-align: center;
    border-style: solid;
    border-width: 1px;
    background: gainsboro;
}

.box header {
    padding: 20px;
    background: gray;
    color: orange;
 
    
}
.boxes{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 200px 200px;
    gap: 35px;
    justify-content:space-evenly;

}

.mern {
  
    background-color:orangered;
    padding-bottom: 150px;
}
 
nav {
    display:flex
}

nav a{
    color: darkgoldenrod;
    padding: 14px 15px;
    text-decoration: underline brown;
    text-align: center;
}

#name{
color: white;
}

aside {
    flex: 1;
    background-color: green;
    padding: 100px;
    text-align: right;
    float: left;
    ;

}
h4, h5, h6{
    padding-bottom: 250px;
}
