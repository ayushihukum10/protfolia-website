This is an HTML code for a personal portfolio website. Here's a breakdown of the different sections and elements:

Head Section

The title of the website is set to "Portfolio Website".
Two external stylesheets are linked: Font Awesome for icons and Google Fonts for the Roboto font family.
A internal stylesheet is defined, which includes styles for various elements such as the body, navbar, container, content, profile picture, and social icons.
Body Section

The navbar is defined, which includes five links: HOME, WORK, ABOUT, PROJECT, and SERVICE. The active link is styled differently.
The main content is divided into four sections: HOME, WORK, ABOUT, and PROJECT.
Each section has a container element that includes a content element, which contains headings, paragraphs, and links.
The HOME section includes a profile picture and a brief introduction.
The WORK section lists the student's educational background.
The ABOUT section lists the student's personal details.
The PROJECT section lists two projects: Bank Management System and Employee Management System.
Social icons are fixed to the left side of the screen, including links to Facebook, LinkedIn, Twitter, and a cube icon.
Styles

The website has a dark background color (#1a1a1a) and white text color.
The navbar has a centered layout with padding and a dark background color.
The content elements have a max-width of 50% and are styled with a font size of 18px and color #b0b0b0.
The profile picture is styled with a border radius of 50% and a border color of #00bcd4.
The social icons are styled with a fixed position, top 50%, and left 20px, with a transform to center them vertically.
Overall, this is a simple and clean portfolio website that showcases the student's personal and educational background, as well as their projects.

code of this is
<html>
 <head>
  <title>
   Portfolio Website
  </title>
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&amp;display=swap" rel="stylesheet"/>
  <style>
   body {
            margin: 0;
            font-family: 'Roboto', sans-serif;
            background-color: #1a1a1a;
            color: #fff;
        }
        .navbar {
            display: flex;
            justify-content: center;
            padding: 20px;
            background-color: #1a1a1a;
        }
        .navbar a {
            color: #fff;
            text-decoration: none;
            margin: 0 15px;
            font-size: 18px;
            position: relative;
        }
        .navbar a:hover::after, .navbar a.active::after {
            content: '';
            position: absolute;
            width: 100%;
            height: 2px;
            background-color: #fff;
            bottom: -5px;
            left: 0;
        }
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 50px;
        }
        .content {
            max-width: 50%;
        }
        .content h1 {
            font-size: 50px;
            color: #00bcd4;
        }
        .content p {
            font-size: 18px;
            color: #b0b0b0;
            margin: 20px 0;
        }
        .content a {
            display: inline-block;
            padding: 10px 20px;
            margin: 10px 10px 10px 0;
            border: 2px solid #00bcd4;
            color: #00bcd4;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s, color 0.3s;
        }
        .content a:hover {
            background-color: #00bcd4;
            color: #1a1a1a;
        }
        .profile-pic {
            position: relative;
        }
        .profile-pic img {
            border-radius: 50%;
            border: 10px solid #00bcd4;
        }
        .social-icons {
            position: fixed;
            top: 50%;
            left: 20px;
            transform: translateY(-50%);
        }
        .social-icons a {
            display: block;
            color: #fff;
            font-size: 24px;
            margin: 10px 0;
            text-decoration: none;
        }
  </style>
 </head>
 <body>
  <div class="navbar">
   <a class="active" href="#">
    HOME
   </a>
   <a href="#">
    WORK
   </a>
   <a href="#">
    ABOUT
   </a>
   <a href="#">
    PROJECT
   </a>
   <a href="#">
    SERVICE
   </a>
  </div>
  <div class="container">
   <div class="content">
    <h1>
     Hi! I Am
     <span style="color: #00bcd4;">
      Ayushi Hukum
     </span>
    </h1>
    <h1>
     Fullstack Developer.
    </h1>
    <p>  My name is Ayushi Hukum, and I'm a student of Artificial Intelligence at Priyadarshini J.L. College of Engineering. I'm eager to learn new skills and explore the exciting field of AI. 
    </p>
    <a href="#">
     Hire Me
    </a>
    <a href="#">
     View Project
    </a>
   </div>
   <div class="profile-pic">
    <img alt="Profile picture of Ayushi Hukum" height="300" src="img1.jpg" width="300"/>
   </div>
  </div>
  <div class="social-icons">
   <a href="#">
    <i class="fab fa-facebook-f">
    </i>
   </a>
   <a href="#">
    <i class="fab fa-linkedin-in">
    </i>
   </a>
   <a href="#">
    <i class="fab fa-twitter">
    </i>
   </a>
   <a href="#">
    <i class="fas fa-cube">
    </i>
   </a>
  </div>
  <div class="container">
   <div class="content">
    <h1>
     Work
    </h1>
    <p>
     Student of Priyadarshini JL College of Engineering
    </p>
    <p>
     Branch: Artificial Intelligence
    </p>
   </div>
  </div>
  <div class="container">
   <div class="content">
    <h1>
     About
    </h1>
    <p>
     <strong>
      Name:
     </strong>
     Ayushi Hukum
    </p>
    <p>
     <strong>
      Address:
     </strong>
     New Nandanvan
    </p>
    <p>
     <strong>
      Contact No.:
     </strong>
     12345678
    </p>
    <p>
     <strong>
      DOB:
     </strong>
     10/08/2002
    </p>
   </div>
  </div>
  <div class="container">
   <div class="content">
    <h1>
     Project
    </h1>
    <p>
     Project 1: Bank Management System
    </p>
    <p>
     Project 2: Employee Management System
    </p>
   </div>
  </div>
 </body>
</html>
