<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stylish Full-Featured Web Page</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f5f5f5;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
        }

        h1 {
            color: #333;
            text-align: center;
            margin-bottom: 20px;
        }

        button {
            padding: 12px;
            background-color: #4caf50;
            color: white;
            border: none;
            cursor: pointer;
            font-size: 16px;
        }

        button:hover {
            background-color: #45a049;
        }

        form {
            text-align: center;
            margin-top: 20px;
        }

        label {
            font-size: 18px;
            color: #555;
        }

        input {
            padding: 10px;
            font-size: 16px;
        }

        #dynamicContent {
            margin-top: 20px;
            font-size: 18px;
            color: #777;
        }
    </style>
</head>
<body>

<h1>Welcome to the Stylish Full-Featured Web Page</h1>

<button onclick="displayMessage()">Click me for an Alert!</button>

<p id="dynamicContent">This content can be updated dynamically.</p>

<form>
    <label for="name">Enter your name:</label>
    <input type="text" id="name" name="name">
    <button type="button" onclick="greetUser()">Greet Me</button>
</form>

<script>
    function displayMessage() {
        alert('Hello! This is an example of HTML integrated with JavaScript.');
    }

    function greetUser() {
        const userName = document.getElementById('name').value;
        alert('Hello, ' + userName + '! Welcome to the Stylish Full-Featured Web Page.');
        document.getElementById('dynamicContent').innerHTML = 'Dynamic content updated for ' + userName + '.';
    }
</script>

</body>
</html>
