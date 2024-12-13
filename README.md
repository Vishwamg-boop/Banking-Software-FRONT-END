# Banking-Software-FRONT-END

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Banking Software</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
        }
        header {
            background-color: #004d99;
            color: #fff;
            padding: 1rem;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: space-around;
            background-color: #003366;
            padding: 0.5rem;
        }
        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }
        .container {
            max-width: 1200px;
            margin: 2rem auto;
            padding: 1rem;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        .form-section {
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }
        label {
            font-weight: bold;
        }
        input, select, button {
            padding: 0.5rem;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        button {
            background-color: #004d99;
            color: white;
            font-size: 1rem;
            cursor: pointer;
        }
        button:hover {
            background-color: #003366;
        }
        footer {
            text-align: center;
            background-color: #004d99;
            color: white;
            padding: 1rem;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Indian Banking Software</h1>
    </header>

    <nav>
        <a href="#dashboard">Dashboard</a>
        <a href="#transactions">Transactions</a>
        <a href="#services">Services</a>
        <a href="#support">Support</a>
        <a href="#logout">Logout</a>
    </nav>

    <div class="container">
        <h2>Login</h2>
        <form class="form-section" id="loginForm">
            <label for="account">Account Number:</label>
            <input type="text" id="account" name="account" placeholder="Enter your account number" required>

            <label for="password">Password:</label>
            <input type="password" id="password" name="password" placeholder="Enter your password" required>

            <button type="submit">Login</button>
        </form>
    </div>

    <footer>
        <p>&copy; 2024 Indian Banking Solutions. All rights reserved.</p>
    </footer>

    <script>
        document.getElementById('loginForm').addEventListener('submit', function(event) {
            event.preventDefault();
            const account = document.getElementById('account').value;
            const password = document.getElementById('password').value;

            if (account && password) {
                alert('Login successful!');
                // Add additional authentication logic here
            } else {
                alert('Please fill out all fields.');
            }
        });
    </script>
</body>
</html>
