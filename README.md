<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Back-End Programming Languages</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron&family=Roboto:wght@300;400;700&display=swap');

        body {
            font-family: 'Orbitron', sans-serif;
            text-align: center;
            margin: 0;
            background: linear-gradient(135deg, #1a1a2e, #16213e, #0f3460);
            color: white;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .container {
            width: 90%;
            max-width: 800px;
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.3);
        }

        .banner {
            width: 100%;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        ul {
            list-style-type: none;
            padding: 0;
        }

        li {
            background: #e94560;
            color: white;
            margin: 10px;
            padding: 15px;
            border-radius: 5px;
            cursor: pointer;
            transition: transform 0.3s, background 0.3s;
            font-size: 18px;
        }

        li:hover {
            background: #ff2e63;
            transform: scale(1.05);
        }

        .description {
            display: none;
            background: rgba(255, 255, 255, 0.2);
            padding: 10px;
            margin-top: 5px;
            border-radius: 5px;
            color: #f1f1f1;
            font-size: 16px;
            font-family: 'Roboto', sans-serif;
        }

        @media (max-width: 600px) {
            body {
                padding: 10px;
            }

            .container {
                padding: 15px;
            }

            li {
                font-size: 16px;
                padding: 10px;
            }

            .description {
                font-size: 14px;
            }
        }
    </style>
</head>

<body>
    <div class="container">
        <h2>Group Members</h2>
        <p><strong>Leader:</strong> Vonzer L. Villamer</p>
        <p><strong>Members:</strong> Verjohn Dave Clarito, Joshua Vargas, Jimuel Quintas, Joana Joyce Barbadillo</p>

        <h3>Background</h3>
        <p>This project aims to provide an overview of key back-end programming languages that are essential for building robust and efficient applications.</p>

        <h3>Programming Languages</h3>
        <p>Click on each language to reveal more details.</p>

        <ul id="languages">
            <li onclick="toggleDescription(0)">C<div class="description">A general-purpose, high-level programming language used for system software, operating systems, and embedded systems.</div></li>
            <li onclick="toggleDescription(1)">Visual Basic<div class="description">A programming language designed for developing Windows applications, with a focus on user interfaces.</div></li>
            <li onclick="toggleDescription(2)">VBScript<div class="description">A scripting language developed by Microsoft, often used for automating tasks in Windows environments.</div></li>
            <li onclick="toggleDescription(3)">Q<div class="description">A functional programming language known for its concise syntax and powerful query capabilities, often used for handling large datasets.</div></li>
            <li onclick="toggleDescription(4)">Bash<div class="description">A command language interpreter for the GNU operating system, widely used for writing shell scripts and automating tasks.</div></li>
            <li onclick="toggleDescription(5)">Java<div class="description">A widely used, object-oriented programming language known for its portability, used in enterprise applications, web development, and Android apps.</div></li>
            <li onclick="toggleDescription(6)">Vyper<div class="description">A Pythonic programming language designed for Ethereum smart contracts, focusing on security and simplicity.</div></li>
            <li onclick="toggleDescription(7)">JavaScript (Node.js)<div class="description">A runtime environment for executing JavaScript on the server-side, used in modern web development.</div></li>
            <li onclick="toggleDescription(8)">Vue.js<div class="description">A progressive JavaScript framework that can be used for backend development with Nuxt.js.</div></li>
            <li onclick="toggleDescription(9)">JHipster<div class="description">A development platform that generates, deploys, and manages Spring Boot and Angular/React/Vue-based applications.</div></li>
        </ul>
    </div>

    <script>
        function toggleDescription(index) {
            let descriptions = document.querySelectorAll('.description');
            descriptions[index].style.display = descriptions[index].style.display === 'block' ? 'none' : 'block';
        }
    </script>
</body>
</html>
