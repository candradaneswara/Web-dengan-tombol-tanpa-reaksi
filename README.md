<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Sans-Serif;
        }
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: black;
        }
        nav a {
            position: relative;
            font-size: 1.1em;
            font-weight: 500;
            color: #333;
            text-decoration: none;
            padding: 6px 20px;
            transition: .5s;
        }
        nav a:hover {
            color: aqua;
        }
        nav a span {
            position: absolute;
            top: 100%;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            border-bottom: 2px solid #0ef;
            border-radius: 15px;
            transform: scaleY(0) translateY(50px);
            opacity: 0;
            transition: 1s;
        }
        nav a:hover span {
            transform: scaleY(1) translateY(0);
            opacity: 1;
        }
        p {
            color: white;
        }
    </style>
</head>
<body>
    <nav>
        <a href="#">home<span></span></a>
        <a href="#">about<span></span></a>
        <a href="#">service<span></span></a>
        <a href="#">contact<span></span></a>
        <a href="#">help<span></span></a>
    </nav>
</body>
</html>
