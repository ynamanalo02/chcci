<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Website</title>
    <style>
        
        #signin-modal {
            display: none;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            z-index: 9999;
        }
        #signin-form {
            background-color: #fff;
            padding: 20px;
            border-radius: 5px;
        }
        #signin-form input[type="text"] {
            margin-bottom: 10px;
        }
    </style>
</head>

<script>
        let userSignedIn = false;

    document.addEventListener('DOMContentLoaded', function() {
        
        const signinModal = document.getElementById('signin-modal');
        const signinForm = document.getElementById('signin-form');
        
        const mainContent = document.getElementById('main-content');

       
        document.body.style.overflow = 'hidden';

        
        signinForm.addEventListener('submit', function(event) {
            event.preventDefault();
            
            const username = document.getElementById('username').value.trim();
            if (username !== '') {
                
                signinModal.style.display = 'none';
               
                userSignedIn = true;
               
                mainContent.style.display = 'block';
               
                document.body.style.overflow = '';
            }
        });
    });
</script>

</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Concepcion Holy Cross College Inc.</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            color: #333;       
  }

        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: rgba(255, 255, 255, 0.8); 
            padding: 20px;
            box-sizing: border-box;
            display: flex;
            justify-content: space-between;
            align-items: center;
            z-index: 1; 
        }

        header h1 {
            font-size: 24px;
            font-family: "Times New Roman", Times, serif;
            font-weight: bold;
            text-transform: uppercase;
            margin: 0;
        }

        .school-logo {
            width: 80px;
            height: auto;
            margin-right: 10px; 
        }

        .title-container {
            display: flex;
            align-items: center;
        }

        nav {
            font-size: 14px;
            display: flex;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
            margin: 0;
            display: flex;
            align-items: center; 
        }

        nav ul li {
            margin-left: 20px;
            position: relative;
        }

        nav ul li a {
            color: black; 
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
            padding: 10px 15px; 
        }

        nav ul ul {
            display: none;
            position: absolute;
            background-color: darkblue;
            padding: 10px;
            margin-top: 5px;
            list-style-type: none; 
        }

        nav ul li:hover ul {
            display: block;
        }

        nav ul li:hover > a {
            color: black;
            background-color: grey;             border-radius: 5px;
        }

        nav ul li ul li:hover a {
            background-color: transparent;
            color: blue; 
        }

        section#home {
            width: 100%;
            height: 100vh; 
            background-image: url('https://i.imgur.com/KWSJBA8.jpeg');
            background-size: cover;
            background-position: center;
            position: relative;
            z-index: 0; 
            overflow-y: auto; 
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            text-align: center;
            position: relative;
            z-index: 1; 
            color: black; 
        }

        h2 {
            font-family: 'Playfair Display', serif;
            font-size: 48px;
            font-weight: 700;
            margin-bottom: 20px;
        }
    
        header {
            transition: background-color 0.3s, box-shadow 0.3s;
        }
        header.scrolled {
            background-color: #fff;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
    </style>
</head>
<body>
    <header>
        <div class="title-container">
            <img src="https://i.imgur.com/DH29mHe.png" alt="School Logo" class="school-logo">
            <h1>Concepcion Holy Cross College Inc.</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#">About Us</a>
                    <ul>
                        <li><a href="#history">History</a></li>
                        <li><a href="#official">Official Statement</a></li>
                        <li><a href="#mission">Mission</a></li>
                        <li><a href="#vision">Vision</a></li>
                        <li><a href="#departments">Departments & Head Teachers</a></li>
                    </ul>
                </li>
                <li><a href="#">Academics</a>
                    <ul>
                        <li><a href="#basic">Basic Education</a></li>
                        <li><a href="#college">College</a></li>
                    </ul>
                </li>
                <li><a href="#">Admissions</a>
                    <ul>
                        <li><a href="#enrollment">How to Enroll</a></li>
                    </ul>
                </li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="#updates">Updates</a></li>
            </ul>
        </nav>
    </header>

<script>
        // JavaScript for adding scrolled class to header on scroll
        window.addEventListener('scroll', function() {
            var header = document.querySelector('header');
            if (window.scrollY > 0) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }
        });
    </script>

    <section id="home">
        <div class="container">
            <!-- Content here -->
        </div>
    </section>
</body>
</html>

    <section id="about">
        <div class="container">
            <h2>About Us</h2>
            <h3 id="history">History</h3>
            <p>Concepcion Holy Cross College (CHCC), Inc. is a private, Catholic school located in Concepcion Tarlac. Founded in 1995 by Pablo L. Tioseco, Sr. and his daughter, Dr. Raquel T. Sta. Ines, CHCC was established to provide students in Concepcion and neighboring areas the opportunity to earn their degrees without having to travel far. The college initially offered courses in Teacher Education, Computer Science, and Business Administration, including Secretarial courses. Four years later, the preschool and elementary departments were established, further expanding the educational offerings of the institution.</p>

            <h3 id="official">Official Statement</h3>
            <p>The administration is grateful to those who appreciate all its efforts and hard work. For those who have valid concerns, we will address these matters in a proper forum. As an institution imbued with public interest, we have grown receptive of criticisms in the appropriate context that aid in the development and progress of the institution and ultimately for the benefit of our students. Rest assured that the institution will serve and respond accordingly. However, accusations that are factually inaccurate and intended solely to malign the institution will be dealt with accordingly. The administration and all of its community will continue to give credit where it is due, and accord respect to those who deserve it.</p>

            <h3 id="mission">Mission:</h3>
            <p>To become a leading God-centered learning institution focused on holistic education that forms and educates individuals to become conscientious, competent, compassionate, and committed persons towards the development of a just and humane society.</p>

            <h3 id="vision">Vision:</h3>
            <p>Holy Cross Concepcion College Inc., is an institution for academic and values formation offering relevant, learner-centered, and values-oriented programs that produce competent persons of character in the service of society. These mission and vision statements serve as guiding principles for our institution, reflecting our commitment to excellence, holistic development, and service to the community.</p>

            <h3 id="departments">Departments & Head Teachers:</h3>
            <table>
                <thead>
                    <tr>
                        <th>Departments</th>
                        <th>Head Teachers</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Elementary</td>
                        <td>Sir Dennis D. Santos</td>
                    </tr>
                    <tr>
                        <td>Junior High School</td>
                        <td>Teacher Angeline G. Zerrudo</td>
                    </tr>
                    <tr>
                        <td>Senior High School</td>
                        <td>Teacher Angeline G. Zerrudo</td>
                    </tr>
                    <tr>
                        <td>College</td>
                        <td>For inquiries for Admin College Office, look for the registrar</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>

    <section id="academics">
        <div class="container">
            <h2>Academics</h2>
            <h3 id="basic">Basic Education:</h3>
            <ul>
                <li>Preschool</li>
                <li>Kindergarten</li>
                <li>Grade 1 to 6</li>
                <li>Grade 7-10 (Junior High School)</li>
                <li>Grade 11-12 (Senior High School)</li>
            </ul>

            <h3 id="college">College:</h3>
            <ul>
                <li>Bachelor in Elementary Education</li>
                <li>Bachelor Secondary Education</li>
                <li>Bachelor of Science in Accountancy</li>
                <li>Bachelor of Science in Accounting & Information System</li>
                <li>Bachelor of Science in Business Administration</li>
                <li>Bachelor of Science in Computer Science</li>
                <li>Bachelor of Science in Criminology</li>
                <li>Bachelor of Science in Hospitality Management</li>
                <li>Associate in Computer Technology</li>
                <li>Bachelor of Science in Nursing (CHCC)</li>
                <li>Bachelor of Science in Medical Technology (CHCC) - SOON</li>
                <li>Bachelor of Science in Civil Engineering (HCC)</li>
            </ul>
        </div>
    </section>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Admissions Process</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f2f2f2;
        }

        .container {
            max-width: 800px;
            margin: 20px auto;
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        h2 {
            color: #333;
            text-align: center;
            margin-bottom: 20px;
        }

        h3 {
            color: #666;
            margin-bottom: 10px;
        }

        ol {
            list-style-type: none;
            counter-reset: steps;
        }

        li {
            counter-increment: steps;
            margin-bottom: 20px;
        }

        li::before {
            content: counter(steps);
            background-color: #007bff;
            color: #fff;
            font-weight: bold;
            border-radius: 50%;
            width: 30px;
            height: 30px;
            display: inline-flex;
            justify-content: center;
            align-items: center;
            margin-right: 10px;
        }

        h4 {
            color: #007bff;
            margin-bottom: 10px;
        }

        p {
            margin: 0 0 10px;
        }
        
       
        nav {
            background-color: #007bff;
            color: #fff;
            padding: 10px 20px;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        nav h2 {
            margin: 0;
            font-size: 1.2em; 
        }

        nav ul {
            list-style-type: none;
            padding: 0;
            margin: 0;
        }

        nav ul li {
            display: inline;
            margin-right: 10px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: bold;
        }

        nav ul li a:hover {
            text-decoration: underline;
        }

        
        footer {
            text-align: center;
            color: #666;
            margin-top: 20px;
            padding-top: 10px;
            border-top: 1px solid #ccc;
            font-size: 0.8em; 
        }
    </style>
</head>
<body>
       <div class="container">
        <h2>Admissions</h2>
        <h3 id="enrollment">Regular Enrollment Process:</h3>
        <ol>
            <li>
                <h4>Assessment</h4>
                <p>Procedure:</p>
                <ol type="a">
                    <li>Check for the courses/subjects to be taken for the current semester</li>
                    <li>Fill-out Assessment Form Including assignment of Section</li>
                    <li>Sign Enrollment Stub</li>
                    <li>Instruct to proceed to the registrar for verification and encoding of subjects/courses</li>
                </ol>
            </li>
            <li>
                <h4>Verification and Recording of Courses/Subjects</h4>
                <p>Procedure:</p>
                <ol type="a">
                    <li>Verify the courses/subjects in the Assessment Form</li>
                    <li>Encode courses/subjects in the system for the COR</li>
                    <li>Sign Enrollment Stub</li>
                    <li>Instruct to proceed to the cashier for payment</li>
                </ol>
            </li>
            <li>
                <h4>Payment</h4>
                <p>Procedure:</p>
                <ol type="a">
                    <li>Collect the amount of P2,000.00 for registration and P5,000.00 for balances</li>
                    <li>Sign Enrollment Stub</li>
                    <li>Instruct to proceed to the Registrar for the printing of the COR</li>
                </ol>
            </li>
            <li>
                <h4>Printing of COR and Officializing Enrollment</h4>
                <p>Procedure:</p>
                <ol type="a">
                    <li>Print the COR</li>
                    <li>Officialize enrollment with seal</li>
                    <li>Sign Enrollment Stub</li>
                    <li>Instruct to proceed for ID</li>
                </ol>
            </li>
            <li>
                <h4>ID</h4>
                <p>Procedure:</p>
                <ol type="a">
                    <li>Check student's information (student shall verify all provided information)</li>
                    <li>Taking of picture</li>
                    <li>Print ID</li>
                    <li>Collect the enrollment stub</li>
                </ol>
            </li>
        </ol>
    </div>
    </body>
</html>


    
    <section id="contact">
        <div class="container">
            <h2>Contact Information</h2>
            <p>Contact Us</p>
            <p>Have questions? Would you like to talk to us about your website needs, our services, or our rates? Our site administrators are available Monday through Friday from 7:00 a.m. to 5:00 p.m. or anytime via e-mail. We’d love to hear from you!</p> 
            <h3> Our Headquarters </h3>
            <p>Brgy. Minane Rose Park, 8JCX+CRG, Concepcion, 2316 Tarlac</p>
            <h3>Phone Number</h3>
            <p> (045) 923 0747</p>
            <h3>E-mail</h3>
            <p>If you’d like a no-obligation proposal from Concepcion holy cross college please be sure to request a quote, and we’ll get back to you right away (usually within 48 hours).</p>
            <p>You can also email us at info@chcc.edu.ph with general questions.</p>
        </div>
    </section>

    <section id="updates">
        <div class="container">
            <h2>Updates</h2>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Instagram-like Post</title>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css"> 
<style>
    body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
    }
    .container {
        max-width: 600px;
        margin: 0 auto;
        padding: 20px;
    }
    .post {
        margin-bottom: 20px;
        position: relative;     }
    .post img {
        max-width: 100%;
        height: auto;
        margin-bottom: 10px;
    }
    .caption {
        font-size: 16px;
        line-height: 1.5;
        margin-bottom: 10px;
    }
    .post-details {
        font-size: 14px;
        color: #999;
    }
    .like-heart {
        position: absolute;
        top: 10px;
        right: 10px;
        cursor: pointer;
    }
    .like-heart:hover {
        transform: scale(1.2);
    }
    .like-heart.red {
        color: red;
    }
    .comments-section {
        margin-top: 20px;
    }
    .comment {
        margin-bottom: 10px;
        border-bottom: 1px solid #ddd;
        padding-bottom: 10px;
    }
    .comment-text {
        margin-bottom: 5px;
    }
</style>
</head>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Instagram-like Post</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css"> 
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
        }
        .post {
            margin-bottom: 20px;
            position: relative;           
            display: flex;            
            flex-direction: column;
        }
        .post img {
            max-width: 100%;
            height: auto;
            margin-bottom: 10px;
        }
        .caption {
            font-size: 16px;
            line-height: 1.5;
            margin-bottom: 10px;
        }
        .post-details {
            font-size: 14px;
            color: #999;
            margin-bottom: 10px; 
        }
        .like-heart {
            align-self: flex-end; 
            cursor: pointer; 
        }
        .like-heart:hover {
            transform: scale(1.2);
        }
        .like-heart.red {
            color: red;
        }
    </style>
</head>
<body>

<section id="updates">
    <div class="container">
        <div class="post">
            <img src="https://i.imgur.com/c2LfDwJ.jpeg" alt="Heartstrings" />
            <p class="caption">Prepare to be enchanted by the heartbeat of emotions! The Student Body Organization, in collaboration with the High School Band and Dance Troupe, proudly presents "Heartstrings", a mesmerizing fusion of our school's spirit into an unforgettable celebration of love. 💖✨ Whether you're single, taken, or somewhere in between, "Heartstrings" invites everyone to embrace camaraderie and connection. Join us to revel in the joy of friendship, the excitement of new encounters, or the comfort of companionship amidst the enchanting ambiance of love.</p>
            <div class="post-details">
                <span class="date">Date: February 15, 2024</span>
                <span class="time">Time: 1:30 PM</span>
                <span class="location">Location: 3rd Floor Montessori Gymnasium</span>
            </div>
            <i class="like-heart fas fa-heart"></i> 
        </div>

        <div class="post">
            <img src="https://i.imgur.com/V9CmPUK.jpeg" alt="Valentine's Day" />
            <p class="caption">🌹 I wanna be your vacuum cleaner, Breathing in your dust, I wanna be your Ford Cortina, I will never rust..  As Valentine's Day approaches, can you sense the gentle whispers of love in the air? We're listening, Crossians! Get ready to immerse yourself in affection and groove to the rhythm of romance, because something truly special is on the horizon! 💖✉️</p>
            <div class="post-details">
                <span class="date">Date: February 8, 2024</span>
            </div>
            <i class="like-heart fas fa-heart"></i>             
        </div>

        <div class="post">
            <img src="https://i.imgur.com/09iBLsS.jpeg" alt="SHS Work Immersion Pinning Ceremony" />
            <p class="caption">🎓 𝐒𝐇𝐒 𝐖𝐨𝐫𝐤 𝐈𝐦𝐦𝐞𝐫𝐬𝐢𝐨𝐧 𝐏𝐢𝐧𝐧𝐢𝐧𝐠 𝐂𝐞𝐫𝐞𝐦𝐨𝐧𝐲 𝟐𝟎𝟐𝟒 🌟 Get ready to witness a monumental moment in the Senior High School journey! Our Grade 12 students are poised for an extraordinary milestone as they prepare for their Pre-Deployment Work Immersion Pinning Ceremony! Let's come together to commemorate their dedication, growth, and the exciting adventures awaiting them. As they venture into the dynamic world beyond the classroom, let's applaud their resilience and enthusiasm for embracing the challenges ahead!</p>
            <div class="post-details">
                <span class="date">Date: January 26, 2024</span>
            </div>
            <i class="like-heart fas fa-heart"></i>             
        </div>

        <div class="post">
                <img src="https://i.imgur.com/kNIdkou.jpeg" alt="Digital Responsibility" />
                <p class="caption">Promoting Responsibility in the Digital Community Join us in the effort to combat fake news! Remember to pause and reflect before sharing. Your dedication to responsible digital citizenship plays a crucial role in fostering a trustworthy online environment. Let's work together to cultivate a culture of credibility and integrity!</p>
                <div class="post-details">
                    <span class="date">Date: January 8, 2024</span>
                </div>
                <i class="like-heart fas fa-heart"></i> 
            </div>

            <div class="post">
                <img src="https://i.imgur.com/2fBmQfy.jpeg" alt="Color Fun Run" />
                <p class="caption">🎨 𝐂𝐎𝐋𝐎𝐑 𝐅𝐔𝐍 𝐑𝐔𝐍 𝟒: 𝐂𝐨𝐥𝐨𝐫 𝐄𝐱𝐩𝐥𝐨𝐬𝐢𝐨𝐧 🎉 Prepare to dive into a wave of colors for a meaningful cause at the Color Fun Run "𝐑𝐮𝐧 𝐨𝐫 𝐃𝐲𝐞 𝟒"! Each stride you make adds vibrancy to our community, as all proceeds will support our outreach and gifting initiatives. Join us in spreading happiness and color across the neighborhood! 🌈 This event is open to everyone, including guests from afar! Secure your tickets at the Montessori Lobby or seek assistance from any S.B.O Officers. 🗓️ Date: December 16, 2023 🕔 Time: 5:00 AM 📝 Registration: Opens at 4:00 AM 📍 Location: CHCCI School Grounds 💸 Tickets: 175 PHP Tickets are available during the following times: 9:00 AM - 9:30 AM 11:30 AM - 1:00 PM 1:45 PM - 2:30 PM 3:15 PM - 4:30 PM</p>
                <div class="post-details">
                    <span class="date">Date: December 16, 2023</span>
                </div>
                <i class="like-heart fas fa-heart"></i> 
       
       
    </div>
</section>

<script>
    document.addEventListener('DOMContentLoaded', function() {
        const likeHearts = document.querySelectorAll('.like-heart');
        likeHearts.forEach(heart => {
            heart.addEventListener('click', function() {
                this.classList.toggle('red');
            });
        });
    });
</script>

</body>
</html>

    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Website</title>
    <style>
        #signin-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            z-index: 9999;
            justify-content: center;
            align-items: center;
        }
        #signin-form {
            background-color: #fff;
            padding: 20px;
            border-radius: 5px;
        }
        #signin-form input[type="text"] {
            margin-bottom: 10px;
        }
        body.no-scroll {
            overflow: hidden;
        }
        #comments {
            margin-top: 20px;
        }
        .comment {
            margin-bottom: 15px;
            border-bottom: 1px solid #ccc;
            padding-bottom: 10px;
        }
        .comment-username {
            font-size: 14px;
            color: #666;
        }
        .comment-text {
            font-size: 16px;
        }
        .comment-time {
            font-size: 12px;
            color: #999;
        }
    </style>
</head>
<body>

<div id="signin-modal">
    <form id="signin-form">
        <h2>Welcome</h2>
        <label for="username">Username:</label><br>
        <input type="text" id="username" required><br>
        <button type="submit">Submit</button>
    </form>
</div>

<div id="main-content">
    <form id="comment-form">
        <textarea id="comment-text" rows="3" placeholder="Write your comment here"></textarea><br>
        <button type="submit">Post Comment</button>
    </form>
    <div id="comments"></div>
</div>

<script>
    document.addEventListener('DOMContentLoaded', function() {
        const username = localStorage.getItem('username');
        if (!username) {
            showSignInModal();
        } else {
            displayUsername(username);
            showCommentsSection();
            fetchComments();         }
    });

    function showSignInModal() {
        const signinModal = document.getElementById('signin-modal');
        signinModal.style.display = 'flex';
        document.body.classList.add('no-scroll');
    }

    const signinForm = document.getElementById('signin-form');
    signinForm.addEventListener('submit', function(event) {
        event.preventDefault();
        const username = document.getElementById('username').value.trim();
        if (username !== '') {
            localStorage.setItem('username', username);
            const signinModal = document.getElementById('signin-modal');
            signinModal.style.display = 'none';
            document.body.classList.remove('no-scroll');
            displayUsername(username);
            showCommentsSection();
        }
    });

    function displayUsername(username) {
        const usernameElement = document.createElement('p');
        usernameElement.textContent = 'Username: ' + username;
        usernameElement.classList.add('comment-username');
        document.getElementById('comments').appendChild(usernameElement);
    }

    function showCommentsSection() {
        document.getElementById('main-content').style.display = 'block';
    }

    const commentForm = document.getElementById('comment-form');
    commentForm.addEventListener('submit', function(event) {
        event.preventDefault();
        const commentText = document.getElementById('comment-text').value.trim();
        if (commentText !== '') {
            const timestamp = new Date().toLocaleString();
            const comment = {
                text: commentText,
                time: timestamp,
                username: localStorage.getItem('username')
            };
            const comments = JSON.parse(localStorage.getItem('comments')) || [];
            comments.push(comment);
            localStorage.setItem('comments', JSON.stringify(comments));
            document.getElementById('comment-text').value = '';
            fetchComments();
        }
    });

    
    function fetchComments() {
        const comments = JSON.parse(localStorage.getItem('comments')) || [];
        const commentsContainer = document.getElementById('comments');
        commentsContainer.innerHTML = '';
        comments.forEach(comment => {
            const newComment = document.createElement('div');
            newComment.classList.add('comment');
            newComment.innerHTML = `
                <p class="comment-text">${comment.text}</p>
                <p class="comment-username">${comment.username}</p>
                <p class="comment-time">${comment.time}</p>
            `;
            commentsContainer.appendChild(newComment);
        });
    }
</script>
