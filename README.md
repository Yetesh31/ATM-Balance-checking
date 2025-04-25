<!DOCTYPE html>

<html lang="en">

<head>

  <meta charset="UTF-8">

  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>ATM Balance Checking</title>

  <style>

    * {

      margin: 0;

      padding: 0;

      box-sizing: border-box;

    }



    body {

      font-family: Arial, sans-serif;

      background-color: #f5f5f5;

      margin: 0;

    }



    .navbar {

      background-color: #00796b;

      overflow: hidden;

      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);

    }



    .navbar a {

      float: left;

      display: block;

      color: white;

      padding: 14px 20px;

      text-align: center;

      text-decoration: none;

      font-size: 18px;

    }



    .navbar a:hover {

      background-color: #004d40;

      color: white;

    }



    .navbar a.active {

      background-color: #004d40;

    }



    .page-content {

      padding: 30px;

      text-align: center;

      color: #333;

    }



    h1 {

      font-size: 36px;

      margin-bottom: 20px;

      color: #00796b;

    }



    h2 {

      font-size: 24px;

      margin-bottom: 10px;

    }



    p {

      font-size: 18px;

      margin-bottom: 20px;

    }



    input[type="text"], input[type="email"], input[type="tel"], input[type="password"] {

      padding: 10px;

      font-size: 18px;

      width: 250px;

      margin-bottom: 20px;

      border: 2px solid #ccc;

      border-radius: 4px;

    }



    button {

      background-color: #4CAF50;

      color: white;

      padding: 10px 20px;

      font-size: 18px;

      border: none;

      border-radius: 4px;

      cursor: pointer;

    }



    button:hover {

      background-color: #45a049;

    }



    .error-message {

      color: red;

      font-size: 18px;

      margin-top: 20px;

    }



    .help-section {

      background-color: #f1f1f1;

      padding: 20px;

      margin-top: 40px;

      border-radius: 8px;

      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);

    }



    .help-section h2 {

      color: #00796b;

      font-size: 28px;

      margin-bottom: 15px;

    }



    .help-section p {

      font-size: 18px;

      color: #333;

    }



    .help-section img {

      width: 100%;

      max-width: 600px;

      margin: 20px 0;

      border-radius: 8px;

    }



    footer {

      text-align: center;

      padding: 10px;

      background-color: #00796b;

      color: white;

      position: fixed;

      bottom: 0;

      width: 100%;

    }



    .page {

      display: none;

    }



    .active {

      display: block;

    }

  </style>

</head>

<body>



  <div class="navbar">

    <a href="javascript:void(0);" onclick="showPage('home')" class="active">Home</a>

    <a href="javascript:void(0);" onclick="showPage('about')">About</a>

    <a href="javascript:void(0);" onclick="showPage('services')">Services</a>

    <a href="javascript:void(0);" onclick="showPage('contact')">Contact</a>

    <a href="javascript:void(0);" onclick="showPage('faq')">FAQ</a>

    <a href="javascript:void(0);" onclick="showPage('signIn')">Sign In</a>

    <a href="javascript:void(0);" onclick="showPage('signUp')">Sign Up</a>

  </div>



  <div class="page-content">

    

    <!-- Home Page -->

    <div id="home" class="page home active">

      <h1>ATM Balance Checking</h1>

      <h2>Welcome to the ATM Balance Checking System</h2>

      <p>To check your balance, please enter your 4-digit PIN below:</p>

      <input type="text" id="pin" maxlength="4" placeholder="Enter your 4-digit PIN" />

      <br/>

      <button onclick="checkPin()">Check Balance</button>

      <div id="errorMessage" class="error-message"></div>



      <div class="help-section">

        <h2>Need Help?</h2>

        <p>If you're having trouble checking your balance, please ensure that you enter the correct 4-digit PIN. If the issue persists, you can reach out to our support team for assistance.</p>

        <img src="https://emerj.com/wp-content/uploads/2018/10/artificial-intelligence-for-atms-6-current-applications-2.jpg" alt="ATM Machine Image" />

        <p>Follow the instructions on the ATM machine to enter your PIN securely and check your balance.</p>

        <button onclick="showPage('contact')">Contact Support</button>

      </div>

    </div>



    <!-- About Page -->

    <div id="about" class="page about">

       <h1>About Us</h1>

      <h2>Who We Are</h2>

      <p>We are a leading provider of online ATM balance checking services. Our platform is designed to provide fast, secure, and reliable access to your financial information from the comfort of your home. We understand the need for privacy, security, and quick access to your bank balance and our solution was built with that in mind. We operate globally, but our roots are in India. Our team consists of passionate engineers, designers, and security experts committed to ensuring that your financial information stays safe.</p>

      <p><strong>Founder:</strong> Batch 5</p>

      <p><strong>Location:</strong> Vadlamudi, Guntur, Andhra Pradesh, India, Vignan University</p>

      <p>Vignan University is located in the heart of Andhra Pradesh, one of the most vibrant educational hubs in South India. The university is known for its top-tier programs in engineering and technology and serves as the backdrop for our innovative solutions.</p>

      <p>Our goal is to bridge the gap between technology and finance by providing an easy-to-use platform for accessing financial details. Whether you're at home, in the office, or on the go, our service gives you instant access to your balance with a simple PIN.</p>

      <p>Our mission is to enhance financial transparency for individuals globally by offering an intuitive and secure platform for balance checks. We are working on continuously improving our service with additional features to make your financial experience even better. Our vision is to expand into new markets and offer new financial tools as we grow.</p>

    </div>



    <!-- Services Page -->

    <div id="services" class="page services">

     <h1>Our Services</h1>

      <h2>What We Offer</h2>

      <p>We offer a range of digital services designed to improve your financial management. Our ATM balance checking system is just the beginning. Below is a list of our core offerings:</p>

      <ul>

        <li><strong>ATM Balance Checking</strong>: With a simple 4-digit PIN, check your balance anytime, anywhere.</li>

        <li><strong>Transaction History</strong>: Review past transactions, so you can track your spending and savings.</li>

        <li><strong>PIN Management</strong>: Change and manage your PIN securely through our platform.</li>

        <li><strong>Account Linking</strong>: Link multiple accounts to access all your balances in one place.</li>

        <li><strong>Security Features</strong>: Multi-factor authentication and encryption to keep your data safe.</li>

        <li><strong>Mobile Access</strong>: Access our services on the go with our mobile-optimized platform.</li>

        <li><strong>24/7 Support</strong>: Our customer support is available round-the-clock to help with any issues.</li>

      </ul>

      <p>Our platform is built with the latest technology to ensure you get a seamless, secure, and efficient experience every time you check your balance or manage your account.</p>

      <p>We are constantly adding new features to meet the needs of our customers, so stay tuned for upcoming updates!</p>    </div>

       </div>



    <!-- FAQ Page -->

    <div id="faq" class="page faq">

      <h1>Frequently Asked Questions (FAQ)</h1>

      <h2>Here are some common questions our users ask:</h2>

      <h3>1. How do I check my balance?</h3>

      <p>Simply enter your 4-digit PIN on the homepage, and you will see your balance instantly.</p>

      <h3>2. What if I forget my PIN?</h3>

      <p>If you've forgotten your PIN, please contact our support team for assistance in resetting it.</p>

      <h3>3. Is my balance information secure?</h3>

      <p>Yes, we use the latest security protocols to ensure that your balance information is protected and encrypted.</p>

    </div>



    <!-- Contact Page -->

    <div id="contact" class="page contact">

      <h1>Contact Us</h1>

      <h2>We'd Love to Hear From You!</h2>

      <p>If you have any questions, feedback, or need assistance, don't hesitate to reach out. Our team is here to help you.</p>

      <p><strong>Email:</strong> support@atmbalancechecker.com</p>

      <p><strong>Phone:</strong> +91 123 456 7890</p>

      <p><strong>Address:</strong> Vignan University, Vadlamudi, Guntur, Andhra Pradesh, India</p>

      <p>Our customer service team is available 24/7. You can email us, call us, or even visit us in person for any help.</p>

      <p>Follow us on social media for the latest updates:</p>

      <ul>

        <li><a href="#">Facebook</a></li>

        <li><a href="#">Twitter</a></li>

        <li><a href="#">Instagram</a></li>

        <li><a href="#">LinkedIn</a></li>

      </ul>

      <h2>Batch Information</h2>

      <p>Batch: 09</p>

      <p>Submitted by:</p>

      <ul>

        <li>231FA04D31 - YETESH -contact number(+91 xxxxxxxxxx)</li>

        <li>231FA04E13 - FOUZIA-contact number(+91 xxxxxxxxxx)</li>

        <li>231FA04E25 – GNANASRI -contact number(+91 xxxxxxxxxx)</li>

        <li>231FA04G75 - NOMESWARI-contact number(+91 xxxxxxxxxx)</li>

       

      </ul>

    </div>



    <!-- Sign In Page -->

    <div id="signIn" class="page signIn">

      <h1>Sign In</h1>

      <h2>Login to Your Account</h2>

      <input type="text" id="signInIdentifier" placeholder="Email" required /><br/>

      <input type="password" id="signInPassword" placeholder="Password" required /><br/>

      <button onclick="signIn()">Sign In</button>

      <div id="signInError" class="error-message"></div>

    </div>



    <!-- Sign Up Page -->

    <div id="signUp" class="page signUp">

      <h1>Sign Up</h1>

      <h2>Create a New Account</h2>

      <input type="text" id="signUpName" placeholder="Full Name" required /><br/>

      <input type="email" id="signUpEmail" placeholder="Email" required /><br/>

      <input type="password" id="signUpPassword" placeholder="Password" required /><br/>

      <button onclick="signUp()">Sign Up</button>

      <div id="signUpError" class="error-message"></div>

    </div>



  </div>



  <footer>

    <p>ATM Balance Checking System - Batch 09| All Rights Reserved</p>

  </footer>



  <script>

    const users = [];

    let loggedInUser = null;



    function showPage(pageId) {

      const pages = document.querySelectorAll('.page');

      pages.forEach(page => page.classList.remove('active'));

      document.getElementById(pageId).classList.add('active');



      const navLinks = document.querySelectorAll('.navbar a');

      navLinks.forEach(link => link.classList.remove('active'));

      document.querySelector(`.navbar a[href="javascript:void(0);"][onclick="showPage('${pageId}')"]`).classList.add('active');

    }



    function signUp() {

      const name = document.getElementById("signUpName").value;

      const email = document.getElementById("signUpEmail").value;

      const password = document.getElementById("signUpPassword").value;

      const signUpError = document.getElementById("signUpError");



      if (users.some(user => user.email === email)) {

        signUpError.textContent = "Email is already in use.";

      } else {

        users.push({ name, email, password });

        signUpError.textContent = "";

        alert("Account created successfully! Please sign in.");

        showPage('signIn');

      }

    }



    function signIn() {

      const email = document.getElementById("signInIdentifier").value;

      const password = document.getElementById("signInPassword").value;

      const signInError = document.getElementById("signInError");



      const user = users.find(u => u.email === email && u.password === password);



      if (user) {

        loggedInUser = user;

        signInError.textContent = "";

        alert("Signed in successfully!");

        showPage('home');

      } else {

        signInError.textContent = "Invalid email or password.";

      }

    }



    function checkPin() {

      if (!loggedInUser) {

        document.getElementById("errorMessage").textContent = "Please sign in to check your balance. If you don't have an account, please create one.";

        return;

      }



      const pin = document.getElementById("pin").value;

      const errorMessage = document.getElementById("errorMessage");



      if (pin.length !== 4 || isNaN(pin)) {

        errorMessage.textContent = "Please enter a valid 4-digit PIN.";

      } else {

        errorMessage.textContent = "";

        alert("Your balance is: $1000");

      }

    }

  </script>



</body>

</html>
