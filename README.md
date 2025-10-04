<!--Day 1: Basic HTML Structure Cheatsheet -->
<!--DOCTYPE Declaration -->

<!DOCTYPE html>
<!--Root HTML Tag -->
<html>
<!-- Head Section-->
<head>
<!--Title of the page (appears on browsers tab)-->
<title>My Page</title>
<!-- Meta Tnformation -->
<meta charset="UTF-8"> <!-- Sets character encoding -->
<meta name='description" content=" Basic HTML structure example">
<meta name="keywords" content="HTML, basics, cheatsheet">
<meta name="author" content="Dhanian">
<!-- External CSS Link -->
    <style>
/* Element Selector */
/* Styles all paragraph elements */
/* Text Color */
/* changes text color */
p {
color: blue;
}
/* Background Color */
/* Applies a solid background color */
body {
background-color: lightgray;
}
/* Background Image */
/* Sets an image as background*/
div {
background-image: url("background.jpg");
background-repeat: no repeat; /* Prevent repeating */
background-size: cover;       /*Stretches image to cover element*/
background-position: center;  /*Centers the image */
}
/* Borders */
/* Add border with width, style, and color */
h1 {
   border: 2px solid black;         /* solid border */
}
p {
   border: 3px dashed red;        /* Dashed border */
   }
div {
    border: 4px dotted green;     /* Dotted border */
    }
    
/*--------- Fonts ---------*/
/* Set the font family */
p {
   font-size: Arial, Helvetica, sans-serif; /* Fallback fonts */
}
/* Set the font size */
h1 {
   font-size: 32px; /* can also use em, rem, % */
   }
   /* Make text bold or light */
h2 {
font-weight: bold; /* values: normal, bold, 100-900 */
}
/* Italicize text */
em {
   font-style: italic; /* values: normal, italic, oblique */
   }

   /*--------- Text Spacing --------- */
   /* control line spacing (vertical) */
   p {
      line-height: 1.6; /* times the font size */
      }
    /* space between letters */
    h1 {
       letter-spacing: 2px;
       }
    /* spacing between words */
    h2 {
    word-spacing: 5px;

/* Align text */
 p {   
 text-align: justify; /* values: left, right, center, justify */
    }
p{
   color: blue;
   font-size: 16px;
   }
/* ID Selector */
/* Styles the element with id="header */
  #header{
    background-color: lightgray;
    text-align: center;
  }
/* Class Selector */
/* Styles all elements with Class="button" */
.button {
     background-color: green;
     color: white;
     padding: 10px;
   }
 /* Universal Selector */
 /* Applies styles to all elements */
     *{
        margin: 0;
        padding: 0;
     }
/* Group Selector */
/* Styes multitude elements at once */
  h1, h2, p {
  font-family: Arial, sans-serif;
}
/* Descendant Selector */
/* styles all paragraphs inside div elements */
div p {
     color: darkred;
  }
  </style>
<link rel="stylesheet" href="style.css">
<!-- JavaScript File-->
<script src="script.js"></script>
  </head>
  <!--Body Section -->
  <body>
  <!--Visible content of the web site goes here -->
<!-- Header Section -->
<!-- Usually contains navigation, logo, or introduction -->
<header>
  <h1> My Website </h1>
  <h2> John Doe </h2>
  <p> Frontend Developer</p
<nav>
  <a href="#habout">About</a><br>
  <a href="#projects">Projects</a><br>
  <a href="#contact">Contact</a><br>
 </nav> 
</header>

<!-- About Section -->
<section id="about">
<h2> About Me </h2>
<p>Hello! I am a passionnate developer learning HTML, CSS, and Javascript.I love building, responsive, and user-friendly website. And is all about Big KahMoh and his Big dreams.</p>
</section>

<!-- Projects Section -->
<section id="projects">
<h2>My Projects</h2>
<ul>
  <li> Personal Blog Website </li>
  <li> Simple E-commerce Page </li>
  <li> Portfolio Website </li>
</ul>
</section>

<!-- Highlighted Project as an Article -->
<article> 
<h2> Featured Project: Portfolio Website </h2>
  <p> This project is a simple portfolio page built with HTML. It includes a header, about section, project showcase, and footer with contact information </p>
</article>

<!-- Footer Section -->
<footer id="contact">
  <p>Contact me at: ndumnankam@gmail.com</p>
<p>&copy; 2025 Nankam Ndum. All rights reserved.</p>
</footer>

  <!-- form Container -->
  <!-- action = where the data is sent -->
  <!-- method = how the data is sen (GET or POST) -->
<h2> Simple Form Example </h2>  
<form action="/submit" method="post">

<!-- Text Input -->
<label for= "username"> Username:</label>
<input type="text" to="username" name="username">
<br><br>

<!-- Password Input -->
<label for="password">Password:</label>
<input type="password" id="password" name="password">
<br><br>

<!-- Email Input -->
<label for="email">Email:</label>
<input type="email" id="email" name="email">
<br><br>

<!-- Number Input -->
<label for="age">Age:</label>
<input type="number" id="age" name="age">
<br><br>

<!-- Submit Button -->
<input type="submit" value="Submit">
</form>
  
  <! Example: text, image, links, buttons -->
  <!-- Basic Image -->
  <!-- src = path or URL of the image -->
  <!-- alt = alternative text if image fails to load -->
  <h2> Basic Image Example </h2>
  <img src ="image.jpg" alt="A sample image">
  <!-- Image with width and height -->
  <h2> Image with Dimensions </h2>
  <img src="landscape.jpg" alt="Beautiful landscape" width="300" height="200">
  <!-- External image from a URL -->
  <h2> External Image Example </h2>
  <img src="https://share.google/images/OwaSIfLHjyNFzCjfk" alt="Exampel Website logo">
  <!-- Accessibility tip: always use alt text for screen readers -->
  
  <h1> Main Heading 1 </h1>
  
  <h2> Subheading 2 </h2>
  <!-- Ordered List (ul)-->
  <!-- Display items with bullet points -->
  <h2> Unordered List Example </h2>
  <ul> 
       <li> Apple </li>
       <li> Bananas </li>
       <li> Cherries </li>
  </ul>
<!-- Ordered List (ol)> 
<!-- Display items with numbers (1, 2, 3) -->
<h2> Ordered List Example </h2>
<ol>
      <li> Wake up </li> 
      <li> Brush teeth </li> 
      <li> Have breakfast </li> 
</ol>
<!-- Ordered List with letters -->
<h2> Ordered List with letters </h2>
<ol type="A">
     <li> Fisrt option </li>
     <li> Second option </li>
     <li> Third option </li>
</ol>        
       
  <h3> Smaller heading </h3>
  <h4> Heading Level 4 </h4>
  <h5> Heading Level 5 </h5>
  <h6> Heading Level 6 </h6>
  <!-- Paragraphs -->
  <p>This is the paragraph of text. Paragraph are use to add readable blocks of content.</p>
  <p>Each paragraph is automatically separated with some spacing above and below.</p>
  <!-- Links -->
  <!-- The <a> tag is use for hyperlinks -->
  <a href="https://www.depo.studio/">Visit Depo Website</a> <br>
  <a href="https://codewithdhanian.gumroad.com/l/gzjvj">Check out the the full stack Ebook</a>
  
  </body>
  </html>
  
  
