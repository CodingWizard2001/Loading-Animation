# Loading Animation

This is a simple loading animation created using HTML and CSS. It can be easily integrated into web projects to provide a visually appealing loading experience for users.

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <!-- Title -->
    <title>Wave Loading Animation</title>

    <!-- Link To CSS -->
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="border">
        <div class="inner"></div>
    </div>
</body>
</html>

```

```css

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body{
    min-height: 100vh;
    background-color: #131313;
}
.border{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    width: 250px;
    height: 30px;
    border: 2px solid #fff;
    border-radius: 25px;
    padding: 4px 4px;
}
.inner{
    position: relative;
    width: 0;
    height: 100%;
    background-color: #fff;
    animation: load 5s linear infinite;
    border-radius: 25px;
}
@keyframes load{
    20%{
        width: 16%;
    }
    40%{
        width: 40%;
    }
    50%{
        width: 37%;
        transition-delay: 0.3s;
    }
    100%{
        width: 100%;
    }
}

```