<!DOCTYPE html>
<html lang="en">

<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lab Project 1</title>
</head>

<body>
    <button id="toggleButton">Toggle Style</button>
    <div id="styledElement" style="color: #ff5c77; background-color: #FFFFFF; font-size: 16px;">The test element.</div>
    <script>
        let clicked = false;
        const btn = document.getElementById('toggleButton');
        const element = document.getElementById('styledElement');
        btn.addEventListener("click", function() {
            clicked = !clicked;
            if (!clicked) {
                element.style.color = '#FFFFFF';
                element.style.backgroundColor = '#ff5c77';
                element.style.fontSize = '20px';
            } else {
                element.style.color = '#ff5c77';
                element.style.backgroundColor = '#FFFFFF';
                element.style.fontSize = '16px';
            }
        });
    </script>
</body>

</html>