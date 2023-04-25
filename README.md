<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>corazón con html y css uwu</title>
</head>

<body>
    <div class="heart"></div>
<p>Miau u</p>
</body>

</html>


body {

    margin: 0;
    padding: 0;
    background-color: black;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;  
     
}
       
p{
        background-color: black;
         color: rgb(228, 116, 222);
         font-family:'Times New Roman', Times, serif;
         padding-top: 50px;
       }

.heart {
    height: 70px;
    width: 70px;
    background-color: red;
    position: relative;
    box-shadow: 10px 10px 90px red;
    animation: animHeart .6s linear infinite;
}

@keyframes animHeart {
    0% {
        transform: rotate(-45deg) scale(1.07);
    }

    80% {
        transform: rotate(-45deg) scale(1);
    }

    100% {
        transform: rotate(-45deg) scale(.8);
    }
}


.heart::before {
    content: '';
    position: absolute;
    height: 70px;
    width: 70px;
    background-color: red;
    box-shadow: -10px 10px 90px red;
    top: -50%;
    border-radius: 50%;
}

.heart::after {
    content: '';
    position: absolute;
    box-shadow: 10px -10px 90px red;
    height: 70px;
    width: 87px;
    background-color: red;
    right: -50px;
    border-radius: 50%;
}
