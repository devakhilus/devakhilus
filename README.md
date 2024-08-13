<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Matrix Effect</title>
    <style>
        body {
            margin: 0;
            overflow: hidden;
            background: black;
            color: green;
            font-family: monospace;
        }
        .matrix {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            pointer-events: none;
            overflow: hidden;
        }
        .matrix span {
            position: absolute;
            font-size: 20px;
            opacity: 0.1;
            white-space: nowrap;
        }
        @keyframes drop {
            0% { transform: translateY(-100%); }
            100% { transform: translateY(100%); }
        }
        .matrix span {
            animation: drop 1s linear infinite;
        }
    </style>
</head>
<body>
    <div class="matrix">
        <span>0</span>
        <span>1</span>
        <span>0</span>
        <span>1</span>
        <span>0</span>
        <span>1</span>
        <!-- Add more spans or make them dynamic with JS if needed -->
    </div>
</body>
</html>
