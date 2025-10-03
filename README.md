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
<link rel="stylesheet" href="style.css">
<!-- JavaScript File-->
<script src="script.js"></script>
  </head>
  <!--Body Section -->
  <body>
  <!--Visible content of the web site goes here -->
  <!-- form Container -->
  <!-- action = where the data is sent -->
  <!-- mwthod = how the data is sen (GET or POST) -->
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
  
  
