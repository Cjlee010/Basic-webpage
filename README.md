# Basic-webpage
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Test Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        h1 {
            color: #4CAF50;
        }
        button {
            padding: 10px 20px;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <h1>Welcome to the Test Page</h1>
    <p>This is a simple HTML page for testing purposes.</p>
    <button onclick="alert('Button clicked!')">Click Me</button>
    <p id="text"></p>
    <input type="text" id="inputField" placeholder="Type something here">
    <button onclick="updateText()">Update Text</button>
    <script>
        function updateText() {
            const input = document.getElementById('inputField').value;
            document.getElementById('text').innerText = `You typed: ${input}`;
        }
    </script>
</body>
</html>
