<?php
// Define the username and password for authentication
$valid_username = 'set_your_username';
$valid_password = 'set_your_password';

// Check if the form is submitted
if ($_SERVER['REQUEST_METHOD'] === 'POST') {
    $username = $_POST['username'];
    $password = $_POST['password'];

    // Validate the username and password
    if ($username === $valid_username && $password === $valid_password) {
        // User is authenticated, show the email form
        showEmailForm();
    } else {
        // Invalid username or password, show an error message
        echo '<div class="container mt-3">
            <div class="alert alert-danger">Invalid username or password.</div>
        </div>';
        showLoginForm();
    }
} else {
    // User has not submitted the form, show the login form
    showLoginForm();
}

function showLoginForm() {
    echo '
    <!DOCTYPE html>
    <html>
    <head>
        <title>Login</title>
        <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    </head>
    <body>
        <div class="container">
            <h2 class="mt-5">Login</h2>
            <form method="post" action="' . $_SERVER['PHP_SELF'] . '">
                <div class="form-group">
                    <label for="username">Username:</label>
                    <input type="text" class="form-control" id="username" name="username" required>
                </div>
                <div class="form-group">
                    <label for="password">Password:</label>
                    <input type="password" class="form-control" id="password" name="password" required>
                </div>
                <button type="submit" class="btn btn-primary">Login</button>
            </form>
        </div>
    </body>
    </html>
    ';
}

function showEmailForm() {
    echo '
    <!DOCTYPE html>
    <html>
    <head>
        <title>Send Email</title>
        <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    </head>
    <body>
        <div class="container">
            <h2 class="mt-5">Send Email</h2>
            <form method="post" action="' . $_SERVER['PHP_SELF'] . '">
                <div class="form-group">
                    <label for="smtpServer">SMTP Server:</label>
                    <input type="text" class="form-control" id="smtpServer" name="smtpServer" required>
                </div>
                <div class="form-group">
                    <label for="port">Port:</label>
                    <input type="number" class="form-control" id="port" name="port" required>
                </div>
                <div class="form-group">
                    <label for="authType">Authentication Type:</label>
                    <select class="form-control" id="authType" name="authType" required>
                        <option value="login">User and Password</option>
                        <!-- Add more options if needed -->
                    </select>
                </div>
                <div class="form-group">
                    <label for="username">Username:</label>
                    <input type="text" class="form-control" id="username" name="username" required>
                </div>
                <div class="form-group">
                    <label for="password">Password:</label>
                    <input type="password" class="form-control" id="password" name="password" required>
                </div>
                <div class="form-group">
                    <label for="from">From:</label>
                    <input type="email" class="form-control" id="from" name="from" required>
                </div>
                <div class="form-group">
                    <label for="to">To:</label>
                    <input type="email" class="form-control" id="to" name="to" required>
                </div>
                <div class="form-group">
                    <label for="subject">Subject:</label>
                    <input type="text" class="form-control" id="subject" name="subject" required>
                </div>
                <div class="form-group">
                    <label for="message">Message:</label>
                    <textarea class="form-control" id="message" name="message" rows="5" required></textarea>
                </div>
                <button type="submit" class="btn btn-primary">Send Email</button>
            </form>
        </div>
    </body>
    </html>
    ';
}
