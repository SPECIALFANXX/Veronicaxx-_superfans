<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fan Club</title>
    <style>
        body { font-family: Arial, sans-serif; }
        .page { display: none; padding: 20px; border: 1px solid #ccc; border-radius: 5px; margin: 20px; }
        .page.active { display: block; }
        .header { text-align: center; font-size: 24px; font-weight: bold; margin-bottom: 20px; }
        #signup { background-color: #f9f9f9; }
        #login { background-color: #e9f7f9; }
        #info { background-color: #f3e9f9; }
        #welcome { background-color: #f9f1e9; }
        #superfan { background-color: #e9f9eb; }
        #membership { background-color: #e9e9f9; }
        #specifications { background-color: #f9e9eb; }
        #confirmation { background-color: #f9e9f3; }
        #payment { background-color: #e9f9f3; }
        #paymentConfirmation { background-color: #f9f9e9; }
        #thankYou { background-color: #e9f9f9; }
    </style>
</head>
<body>

<div id="signup" class="page active">
    <h1>Sign Up</h1>
    <form id="signupForm">
        <label for="signupUsername">Username:</label>
        <input type="text" id="signupUsername" required><br>
        <label for="signupEmail">Email:</label>
        <input type="email" id="signupEmail" required><br>
        <label for="signupPassword">Password:</label>
        <input type="password" id="signupPassword" required>
        <input type="checkbox" id="toggleSignupPassword"> Show Password<br>
        <label for="signupConfirmPassword">Confirm Password:</label>
        <input type="password" id="signupConfirmPassword" required>
        <input type="checkbox" id="toggleSignupConfirmPassword"> Show Password<br>
        <button type="submit">Sign Up</button>
    </form>
</div>

<div id="login" class="page">
    <h1>Login</h1>
    <form id="loginForm">
        <label for="loginUsername">Username:</label>
        <input type="text" id="loginUsername" required><br>
        <label for="loginPassword">Password:</label>
        <input type="password" id="loginPassword" required>
        <input type="checkbox" id="toggleLoginPassword"> Show Password<br>
        <button type="submit">Login</button>
    </form>
</div>

<div id="info" class="page">
    <h1>Information Page</h1>
    <form id="infoForm">
        <label for="fullName">Full Name:</label>
        <input type="text" id="fullName" required><br>
        <label for="dob">Date of Birth:</label>
        <input type="date" id="dob" required><br>
        <label for="gender">Gender:</label>
        <select id="gender" required>
            <option value="">Select Gender</option>
            <option value="male">Male</option>
            <option value="female">Female</option>
            <option value="other">Other</option>
        </select><br>
        <label for="address">Address:</label>
        <input type="text" id="address" placeholder="Street" required><br>
        <input type="text" id="city" placeholder="City" required><br>
        <input type="text" id="state" placeholder="State" required><br>
        <input type="text" id="zip" placeholder="Zip Code" required><br>
        <label for="phone">Phone Number:</label>
        <input type="tel" id="phone" required><br>
        <label for="infoEmail">Email Address:</label>
        <input type="email" id="infoEmail" required><br>
        <button type="submit">Submit</button>
    </form>
</div>

<div id="welcome" class="page">
    <h1>Hello Fan</h1>
    <p>
        Welcome to the Super Fan Club!
        Your passion and support make all the difference, and I'm beyond excited to have you join this exclusive community. Prepare yourself for behind-the-scenes content, early access to new projects, and a closer connection to everything we're building together. Let's create something amazing!
    </p>
    <p>
        Thank you for being an amazing supporter. Let's make this journey unforgettable!
    </p>
    <p>Warm regards</p>
    <button onclick="showPage('superfan')">Next</button>
</div>

<div id="superfan" class="page">
    <h1>❤️‍🔥What my superfans grant ⬇️</h1>
    <p>📍Daily New Content (over 50+ sexy& nudes pics including vids you get immediate access to upon subscription)</p>
    <p>📍B/G and Solo content (PPV)</p>
    <p>📌I sell my panties</p>
    <p>📍Twerk videos</p>
    <p>❣️Video calls</p>
    <p>🥰 Unlimited chat</p>
    <p>❣️Exclusive videos</p>
    <p>❣️Masturbating video</p>
    <p>❣️Random meeting</p>
    <p>📌One-on-one messaging 24/7</p>
    <button onclick="showPage('membership')">Next</button>
</div>

<div id="membership" class="page">
    <h1>Membership Details</h1>
    <form id="membershipForm">
        <label for="membershipType">Choose Membership:</label>
        <select id="membershipType" required>
            <option value="">Membership</option>
            <option value="regular">$250 Regular</option>
        </select><br>
        <label for="communication">Preferred Mode of Communication:</label>
        <select id="communication" required>
            <option value="">Select Communication Mode</option>
            <option value="email">Email</option>
            <option value="phone">Phone</option>
        </select><br>
        <button type="submit">Submit</button>
    </form>
</div>

<div id="specifications" class="page">
    <h1>Fan Club-Specific Information</h1>
    <form id="specificationsForm">
        <label for="hearAbout">How did you hear about the fan club?</label><br>
        <textarea id="hearAbout" required></textarea><br>
        <label for="hopeToGain">What do you hope to gain from joining the fan club?</label><br>
        <textarea id="hopeToGain" required></textarea><br>
        <label for="suggestions">Any suggestions for activities or events:</label><br>
        <textarea id="suggestions" required></textarea><br>
        <button type="submit">Submit</button>
    </form>
</div>

<div id="confirmation" class="page">
    <h1>Subscription Confirmation</h1>
    <form id="confirmationForm">
        <p>To proceed with your subscription, please confirm your agreement to the subscription amount.</p>
        <p>By checking this box, you acknowledge and agree to the annual subscription fee of $250.</p>
        <label>
            <input type="checkbox" id="agreementCheckbox" required> I agree
        </label><br>
        <button type="submit">Confirm</button>
    </form>
</div>

<div id="payment" class="page">
    <h1>Payment Mode</h1>
    <p>Please select your payment method:</p>
    <form id="paymentForm">
        <label>
            <input type="radio" name="paymentMethod" value="Crypto" required> Crypto
        </label><br>
        <div id="paymentInfo"></div>
        <button type="submit">Submit</button>
    </form>
    <button onclick="showPage('paymentConfirmation')">Next</button>
</div>

<div id="paymentConfirmation" class="page">
    <h1>Payment Confirmation</h1>
    <p>Please forward all payment screenshots to the following email address: veronica60641130@gmail.com</p>
    <p>Also upload all payment screenshot below:</p>
    <form id="paymentConfirmationForm">
        <input type="file" accept="image/*" required><br>
        <button type="submit">Upload</button>
    </form>
</div>

<div id="thankYou" class="page">
    <h1>Thank You for Subscribing!</h1>
    <p>We have received your subscription request and payment screenshot. Thank you for subscribing to Super Fans! We will review your submission and provide you with exclusive access shortly.</p>
</div>

<script>
    const users = {};
    const signupForm = document.getElementById('signupForm');
    const loginForm = document.getElementById('loginForm');
    const infoForm = document.getElementById('infoForm');
    const membershipForm = document.getElementById('membershipForm');
    const specificationsForm = document.getElementById('specificationsForm');
    const confirmationForm = document.getElementById('confirmationForm');
    const paymentForm = document.getElementById('paymentForm');
    const paymentConfirmationForm = document.getElementById('paymentConfirmationForm');

    signupForm.addEventListener('submit', function(event) {
        event.preventDefault();
        const username = document.getElementById('signupUsername').value;
        const email = document.getElementById('signupEmail').value;
        const password = document.getElementById('signupPassword').value;
        const confirmPassword = document.getElementById('signupConfirmPassword').value;

        if (password !== confirmPassword) {
            alert('Passwords do not match.');
            return;
        }

        users[username] = { email, password };
        alert('Sign up successful! Please log in.');
        showPage('login');
    });

    loginForm.addEventListener('submit', function(event) {
        event.preventDefault();
        const username = document.getElementById('loginUsername').value;
        const password = document.getElementById('loginPassword').value;

        if (users[username] && users[username].password === password) {
            alert('Login successful!');
            showPage('info');
        } else {
            alert('Invalid username or password.');
        }
    });

    infoForm.addEventListener('submit', function(event) {
        event.preventDefault();
        showPage('welcome');
    });

    membershipForm.addEventListener('submit', function(event) {
        event.preventDefault();
        showPage('specifications');
    });

    specificationsForm.addEventListener('submit', function(event) {
        event.preventDefault();
        showPage('confirmation');
    });

    confirmationForm.addEventListener('submit', function(event) {
        event.preventDefault();
        showPage('payment');
    });

    paymentForm.addEventListener('submit', function(event) {
        event.preventDefault();
        const selectedPaymentMethod = document.querySelector('input[name="paymentMethod"]:checked').value;
        let paymentInfo = '';
        switch (selectedPaymentMethod) {
            case 'Crypto':
                paymentInfo = 'Crypto: 1CzT6CnQpbtgDs6ZafzBHQQP26C9BkyQwH';
                break;
        }
        document.getElementById('paymentInfo').innerText = paymentInfo;
    });

    paymentConfirmationForm.addEventListener('submit', function(event) {
        event.preventDefault();
        alert('Payment screenshot uploaded successfully.');
        showPage('thankYou');
    });

    document.getElementById('toggleSignupPassword').addEventListener('change', function() {
        const passwordInput = document.getElementById('signupPassword');
        passwordInput.type = this.checked ? 'text' : 'password';
    });

    document.getElementById('toggleSignupConfirmPassword').addEventListener('change', function() {
        const passwordInput = document.getElementById('signupConfirmPassword');
        passwordInput.type = this.checked ? 'text' : 'password';
    });

    document.getElementById('toggleLoginPassword').addEventListener('change', function() {
        const passwordInput = document.getElementById('loginPassword');
        passwordInput.type = this.checked ? 'text' : 'password';
    });

    function showPage(pageId) {
        const pages = document.querySelectorAll('.page');
        pages.forEach(page => page.classList.remove('active'));
        document.getElementById(pageId).classList.add('active');
    }
</script>

</body>
</html>
