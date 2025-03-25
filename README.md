# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Page</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: Arial, sans-serif;
        }
        .container {
            display: grid;
            grid-template-rows: auto 1fr auto;
            min-height: 100vh;
        }
        nav {
            background: #333;
            color: white;
            display: flex;
            justify-content: space-between;
            padding: 1rem;
        }
        nav ul {
            list-style: none;
            display: flex;
        }
        nav ul li {
            margin: 0 10px;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
        }
        .content {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
            padding: 20px;
        }
        .box {
            background: lightgray;
            padding: 20px;
            text-align: center;
        }
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 1rem;
        }

        @media (min-width: 600px) {
            .content {
                grid-template-columns: repeat(2, 1fr);
            }
        }
        @media (min-width: 900px) {
            .content {
                grid-template-columns: repeat(3, 1fr);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <nav>
            <div class="logo">Logo</div>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
        <div class="content">
            <div class="box">Box 1</div>
            <div class="box">Box 2</div>
            <div class="box">Box 3</div>
            <div class="box">Box 4</div>
            <div class="box">Box 5</div>
            <div class="box">Box 6</div>
        </div>
        <footer>
            &copy; 2025 Responsive Page
        </footer>
    </div>
</body>
</html>

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨
