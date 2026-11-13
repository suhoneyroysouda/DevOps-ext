
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(135deg, #667eea, #764ba2);
        }

        .login-box {
            width: 350px;
            padding: 35px;
            background: white;
            border-radius: 12px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.2);
        }

        h2 {
            text-align: center;
            margin-bottom: 25px;
            color: #333;
        }

        input {
            width: 100%;
            padding: 12px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 6px;
        }

        button {
            width: 100%;
            padding: 12px;
            margin-top: 15px;
            background: #667eea;
            color: white;
            border: none;
            border-radius: 6px;
            cursor: pointer;
            font-size: 16px;
        }

        button:hover {
            background: #764ba2;
        }

        p {
            text-align: center;
            margin-top: 15px;
            font-size: 14px;
        }

        a {
            color: #667eea;
            text-decoration: none;
        }
    </style>
</head>

<body>

    <div class="login-box">
        <h2>Login</h2>

        <form onsubmit="login(event)">
            <input type="email" placeholder="Enter Email" required>

            <input type="password" placeholder="Enter Password" required>

            <button type="submit">Login</button>
        </form>

        <p><a href="#">Forgot Password?</a></p>
        <p>Don't have an account? <a href="#">Sign Up</a></p>
    </div>

    <script>
        function login(event) {
            event.preventDefault();
            alert("Login button clicked!");
        }
    </script>

</body>
</html>
