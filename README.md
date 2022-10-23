# Glitch-text
HTML
<!DOCTYPE html>
<html>
    <head>
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CustomeValPage</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
    <h1 class="valorant">VALORANT</h1>   
    </body>
</html>

CSS
*{
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
    box-sizing: border-box;
}
body{
    background: #222;
    color: white;
}
.valorant{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 100px;
    letter-spacing: 8px;
    cursor: pointer;
}
.valorant::before,.valorant::after{
    content: 'VALORANT';
    display: block;
    position: absolute;
    top: 0px;
    left: 0px;
}
.valorant:hover::before{
    animation: valorant 0.3s linear 6;
    color: #e91e63;
    z-index: -2;
}
.valorant:hover::after{
    animation: valorant 0.3s linear 6 reverse;
    color: #2196f3;
    z-index: -1;
}
@keyframes valorant{
    0%{
        top: 0;
        left: 0;
    }
    20%{
        top: -5px;
        left: -5px;
    }
    40%{
        top: 5px;
        left: 5px;
    }
    60%{
        top: -5px;
        left: 5px;
    }
    80%{
        top: 5px;
        left: -5px;
    }
    100%{
        top: 0;
        left: 0;
    }
    }
    
