<!DOCTYPE html>
<html>
<head>
    <title>Change Website Color</title>
    <style>
        body {
            transition: background-color 0.5s;
        }
    </style>
</head>
<body>

<h1>Change Website Color</h1>
<p>Click the button to change the background color.</p>

<button id="colorButton">Change Color</button>

<script>
    const colors = ["#FF5733", "#33FF57", "#5733FF", "#33A0FF", "#FF33A0"];
    let currentIndex = 0;

    document.getElementById("colorButton").addEventListener("click", () => {
        document.body.style.backgroundColor = colors[currentIndex];
        currentIndex = (currentIndex + 1) % colors.length;
    });
</script>

</body>
</html>

