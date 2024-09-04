Start a html file with :

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="A brief description of your webpage">
    <title>Your Website Title</title> 
    <link rel="stylesheet" href="styles.css"> <!-- Link to your CSS file -->
</head>
<body>

</body>

anchor (<a>) element, commonly used to create hyperlinks

href="#": specifies the URL of the page the link goes to.
# = placeholder that doesn't link to an external page but rather to the top of the current page 

<nav> element in HTML is used to define a block of navigation links

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css" integrity="sha512-Kc323vGBEqzTmouAECnVceyQqyqdsSiqLQISBL29aUW4U/M7pSPA/gEUZQqv1cwx4OnYxTxve5UMg5GT6L4JJg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
 Font Awesome library, which provides a set of scalable vector icons that you can use on your website


  <section class="experience" id="experience">
        <div class="experience-container">
            <nav class="experience-nav">
                <button class="tablink active" onclick="openTab(event, 'work')">Work Experiences</button>
                <button class="tablink" onclick="openTab(event, 'professional')">Professional Dev Experiences</button>
                <button class="tablink" onclick="openTab(event, 'volunteer')">Volunteer Experiences</button>
            </nav>
    
            <div class="tabcontent" id="work">
                <div class="experience-box">
                    <h3>Software Developer at XYZ Corp</h3>
                    <p>Developed web applications using React and Node.js...</p>
                </div>
                <!-- Add more work experiences here -->
            </div>
    
            <div class="tabcontent" id="professional" style="display:none;">
                <div class="experience-box">
                    <h3>Completed Full-Stack Web Development Course</h3>
                    <p>Learned technologies such as HTML, CSS, JavaScript, and React...</p>
                </div>
                <!-- Add more professional development experiences here -->
            </div>
    
            <div class="tabcontent" id="volunteer" style="display:none;">
                <div class="experience-box">
                    <h3>Volunteer Teacher at Kids Who Code</h3>
                    <p>Taught Python programming to middle school students...</p>
                </div>
                <!-- Add more volunteer experiences here -->
            </div>
        </div>
    </section>
    
    

.experience {
    padding: 50px;
    background-color: #f9f9f9;
}

.experience-container {
    max-width: 800px;
    margin: 0 auto;
    text-align: center;
}

.experience-nav {
    display: flex;
    justify-content: center;
    margin-bottom: 20px;
}

.tablink {
    background-color: #e0e0e0;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    transition: background-color 0.3s;
}

.tablink.active, .tablink:hover {
    background-color: #333;
    color: white;
}

.tabcontent {
    display: none;
}

.tabcontent.active {
    display: block;
}



